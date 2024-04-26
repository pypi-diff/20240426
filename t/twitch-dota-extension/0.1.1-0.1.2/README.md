# Comparing `tmp/twitch_dota_extension-0.1.1.tar.gz` & `tmp/twitch_dota_extension-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch_dota_extension-0.1.1.tar", max compression
+gzip compressed data, was "twitch_dota_extension-0.1.2.tar", max compression
```

## Comparing `twitch_dota_extension-0.1.1.tar` & `twitch_dota_extension-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       58 2024-04-17 16:20:11.616674 twitch_dota_extension-0.1.1/README.md
--rw-r--r--   0        0        0      480 2024-04-22 15:12:20.797015 twitch_dota_extension-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 15:48:53.325498 twitch_dota_extension-0.1.1/twitch_dota_extension/api.py
--rw-r--r--   0        0        0     5841 2024-04-22 15:12:13.588941 twitch_dota_extension-0.1.1/twitch_dota_extension/lib.py
--rw-r--r--   0        0        0     2527 2024-04-18 19:25:34.069698 twitch_dota_extension-0.1.1/twitch_dota_extension/tooltips.py
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 twitch_dota_extension-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       58 2024-04-17 16:20:11.616674 twitch_dota_extension-0.1.2/README.md
+-rw-r--r--   0        0        0      480 2024-04-26 13:49:47.571251 twitch_dota_extension-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7727 2024-04-25 15:56:25.054341 twitch_dota_extension-0.1.2/twitch_dota_extension/lib.py
+-rw-r--r--   0        0        0     2527 2024-04-18 19:25:34.069698 twitch_dota_extension-0.1.2/twitch_dota_extension/tooltips.py
+-rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 twitch_dota_extension-0.1.2/PKG-INFO
```

### Comparing `twitch_dota_extension-0.1.1/twitch_dota_extension/lib.py` & `twitch_dota_extension-0.1.2/twitch_dota_extension/lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,58 +33,64 @@
             if items[slot].name != 'empty':
                 items_.append(itemdef[items[slot].name])
         neutral = itemdef[items["neutral0"].name] if items["neutral0"].name != 'empty' else None
         return Inventory(items_, neutral)
 
 @dataclass
 class HeroData:
-    name: str
     t: list[int]
     items: dict[str, HDItem]
     # base_ability_count: int
 
 @dataclass
+class TournamentHeroData(HeroData):
+    p: str # playername
+    lvl: int
+    aghs: list[int]
+
+@dataclass
 class TalentEntry:
     name: str
     picked: bool
 
 @dataclass
 class TalentTree:
-    entries: list[tuple[TalentEntry]]
+    entries: list[tuple[TalentEntry, TalentEntry]]
 
     @staticmethod
     def from_parts(talents: list[str], picks: list[int]) -> 'TalentTree':
         entries: list[TalentEntry] = []
         for talent, picked in zip(talents, picks):
             entries.append(TalentEntry(name=talent, picked=bool(picked)))
         # TODO: these are backwards in the API!!
         # it returns 0, 1, 2, 3, .. where 0, 2, 4, 6 are RIGHT and 1,3,5,7 are LEFT
         list_of_groups = list(zip(*(iter(entries),) * 2))
         return TalentTree(entries=list_of_groups)
 
 @dataclass
-class ProcessdHeroData:
+class ProcessedHeroData:
     n: str
     name: str
     talent_tree: TalentTree
     abilities: list[Ability]
     inventory: Inventory
+    player: Optional[str] = None
 
 
 @dataclass
 class Playing:
     selected_hero: str
     selected_hero_data: HeroData
 
-    def process_data(self, heroes, items) -> 'ProcessdHeroData':
+    def process_data(self, heroes: dict[str, Hero], items) -> ProcessedHeroData:
         hero = heroes[self.selected_hero]
         talents = TalentTree.from_parts(hero.talents, self.selected_hero_data.t)
         inv = Inventory.from_parts(self.selected_hero_data.items, items)
 
-        phd = ProcessdHeroData(hero.n, hero.name, talents, hero.abilities, inv)
+        phd = ProcessedHeroData(hero.n, hero.name, talents, hero.abilities, inv)
         return phd
 
 
 @dataclass
 class CDNConfig:
     domain: str
 
@@ -92,34 +98,50 @@
     def default() -> "CDNConfig":
         return CDNConfig("dotatooltips.b-cdn.net")
 
 
 @dataclass
 class APIConfig:
     domain: str
+    tour_domain: str
 
     @staticmethod
     def default() -> "APIConfig":
-        return APIConfig("tooltips.layerth.dev")
+        return APIConfig("tooltips.layerth.dev", "tour-tooltips.layerth.dev")
 
 
 @dataclass
 class Spectating:
     heroes: list[str]
-    hero_data: dict[str, Any]
+    hero_data: dict[str, HeroData]
 
 
 @dataclass
+class SpectatingTournament:
+    hero_data: dict[str, TournamentHeroData]
+
+    def process_data(self, heroes: dict[str, Hero], items) -> list[ProcessedHeroData]:
+        ret = []
+        for hero_name, hero_state in self.hero_data.items():
+            hero = heroes[hero_name]
+            talents = TalentTree.from_parts(hero.talents, hero_state.t)
+            inv = Inventory.from_parts(hero_state.items, items)
+
+            phd = ProcessedHeroData(hero.n, hero_name, talents, hero.abilities, inv, player=hero_state.p)
+            ret.append(phd)
+        return ret
+
+@dataclass
 class InvalidResponse:
     r: dict[str, Any]
 
 
 @dataclass
 class APIError:
-    pass
+    error: str
 
 
 class DataType(enum.Enum):
     Items = enum.auto()
     Heroes = enum.auto()
 
 
@@ -161,28 +183,39 @@
             case DataType.Heroes:
                 type_ = "full-heroes"
             case default:
                 raise ValueError(f"Unsupported value {default}")
         url = f"https://{self.cdn_config.domain}/data/{language}/{type_}.json"
         return await self._fetch_json(url)
 
-    async def get_stream_status(self, channel_id: int) -> Playing | APIError | Spectating | InvalidResponse:
+    async def get_stream_status(self, channel_id: int) -> Playing | APIError | Spectating | SpectatingTournament | InvalidResponse:
+        MAYBE_IN_TOURNAMENT = "Channel not found. It might take a few minutes for the channel to appear."
         url = f"https://{self.api_config.domain}/data/pubsub/{channel_id}"
         data = await self._fetch_json(url)
 
-        return API._from_json(data)
+        if data.get('error') == MAYBE_IN_TOURNAMENT:
+            print("Attempting to fetch from tournament domain")
+            url_tour = f"https://{self.api_config.tour_domain}/data/pubsub/{channel_id}"
+            data = await self._fetch_json(url_tour)
+
+        r = API._from_json(data)
+        return r
 
     @staticmethod
-    def _from_json(data: dict) -> Playing | APIError | Spectating | InvalidResponse:
-        assert not data["error"], "not implemented, error management"
+    def _from_json(data: dict) -> Playing | APIError | Spectating | SpectatingTournament | InvalidResponse:
+        error = data.get("error")
+        if error:
+            return APIError(error)
         game = data.get("active_game", {})
         state = game.get("gsi_state", "unpopulated in API")
 
         if state == "playing":
             return dacite.from_dict(data_class=Playing, data=game)
+        elif state == "spectating" and game.get('matchid'):  # Tournament
+            return dacite.from_dict(data_class=SpectatingTournament, data=game)
         elif state == "spectating":
             return dacite.from_dict(data_class=Spectating, data=game)
 
         return InvalidResponse(r=data)
 
 
 
@@ -190,21 +223,32 @@
         def default(self, o):
             if dataclasses.is_dataclass(o):
                 return dataclasses.asdict(o)
             return super().default(o)
 
 
 if __name__ == "__main__":
-    api = API()
-    with Path("./data/playing-2.json").open() as fd:
-        # with Path('./data/spectating.json').open() as fd:
-        # with Path('./data/full-heroes.json').open() as fd:
-        data = json.load(fd)
-
-    heroes = api.fetch_heroes()
-    items = api.fetch_items()
-    game_state = api._from_json(data)
-    match game_state:
-        case Playing():
-            phd = game_state.process_data(heroes, items)
 
-            print(json.dumps(phd, cls=EnhancedJSONEncoder))
+    async def f():
+        api = API()
+        with Path("./data/playing-2.json").open() as fd:
+        #with Path("./data/spectating-tournament.json").open() as fd:
+            # with Path('./data/spectating.json').open() as fd:
+            # with Path('./data/full-heroes.json').open() as fd:
+            data = json.load(fd)
+
+        heroes = await api.fetch_heroes()
+        items = await api.fetch_items()
+        game_state = api._from_json(data)
+        match game_state:
+            case Playing():
+                phd = game_state.process_data(heroes, items)
+                fd = open("data/output/playing.json", 'w')
+                print(json.dumps(phd, cls=EnhancedJSONEncoder), file=fd)
+
+            case SpectatingTournament():
+                phd = game_state.process_data(heroes, items)
+
+                fd = open("data/output/tournament.json", 'w')
+                print(json.dumps(phd, cls=EnhancedJSONEncoder), file=fd)
+    import asyncio
+    asyncio.run(f())
```

### Comparing `twitch_dota_extension-0.1.1/twitch_dota_extension/tooltips.py` & `twitch_dota_extension-0.1.2/twitch_dota_extension/tooltips.py`

 * *Files identical despite different names*

### Comparing `twitch_dota_extension-0.1.1/PKG-INFO` & `twitch_dota_extension-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dota-extension
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interact with the Dota2 Extension API for a given Twitch channel ID
 License: MIT
 Author: David Ventura
 Author-email: davidventura27@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

