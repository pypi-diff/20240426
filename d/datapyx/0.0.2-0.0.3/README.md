# Comparing `tmp/datapyx-0.0.2.tar.gz` & `tmp/datapyx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapyx-0.0.2.tar", last modified: Wed Apr 17 21:42:18 2024, max compression
+gzip compressed data, was "datapyx-0.0.3.tar", last modified: Fri Apr 26 21:03:22 2024, max compression
```

## Comparing `datapyx-0.0.2.tar` & `datapyx-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 21:42:18.483857 datapyx-0.0.2/
--rw-rw-rw-   0        0        0      179 2024-04-17 21:42:18.482884 datapyx-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       28 2024-04-17 19:57:28.000000 datapyx-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 21:42:18.469582 datapyx-0.0.2/datapyx/
--rw-rw-rw-   0        0        0       19 2024-04-17 19:54:48.000000 datapyx-0.0.2/datapyx/__init__.py
--rw-rw-rw-   0        0        0   133199 2024-04-17 21:12:33.000000 datapyx-0.0.2/datapyx/pack.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:42:18.481910 datapyx-0.0.2/datapyx.egg-info/
--rw-rw-rw-   0        0        0      179 2024-04-17 21:42:18.000000 datapyx-0.0.2/datapyx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-04-17 21:42:18.000000 datapyx-0.0.2/datapyx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 21:42:18.000000 datapyx-0.0.2/datapyx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 21:42:18.000000 datapyx-0.0.2/datapyx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2024-04-17 19:58:20.000000 datapyx-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 21:42:18.483857 datapyx-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      371 2024-04-17 21:40:54.000000 datapyx-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 21:03:22.498137 datapyx-0.0.3/
+-rw-rw-rw-   0        0        0      179 2024-04-26 21:03:22.496191 datapyx-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2024-04-17 19:57:28.000000 datapyx-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 21:03:22.485481 datapyx-0.0.3/datapyx/
+-rw-rw-rw-   0        0        0       19 2024-04-17 19:54:48.000000 datapyx-0.0.3/datapyx/__init__.py
+-rw-rw-rw-   0        0        0   140290 2024-04-26 20:59:21.000000 datapyx-0.0.3/datapyx/pack.py
+drwxrwxrwx   0        0        0        0 2024-04-26 21:03:22.496191 datapyx-0.0.3/datapyx.egg-info/
+-rw-rw-rw-   0        0        0      179 2024-04-26 21:03:22.000000 datapyx-0.0.3/datapyx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2024-04-26 21:03:22.000000 datapyx-0.0.3/datapyx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 21:03:22.000000 datapyx-0.0.3/datapyx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 21:03:22.000000 datapyx-0.0.3/datapyx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2024-04-17 19:58:20.000000 datapyx-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 21:03:22.498137 datapyx-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      371 2024-04-26 20:59:34.000000 datapyx-0.0.3/setup.py
```

### Comparing `datapyx-0.0.2/datapyx/pack.py` & `datapyx-0.0.3/datapyx/pack.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,14 +219,58 @@
 df = pd.read_json('./output.json')
 
 #Print first 5 entries
 df.head()
 
 
 2.6 Loading From SQL
+
+SQL:
+CREATE DATABASE movies;
+
+USE movies;
+
+CREATE TABLE movie (
+    movie_id INT PRIMARY KEY,
+    title VARCHAR(255),
+    budget INT,
+    homepage VARCHAR(255),
+    overview TEXT,
+    popularity FLOAT,
+    release_date DATE,
+    revenue BIGINT,
+    runtime INT,
+    movie_status VARCHAR(50),
+    tagline VARCHAR(255),
+    vote_average FLOAT,
+    vote_count INT
+);
+
+
+INSERT INTO movie (movie_id, title, budget, homepage, overview, popularity, release_date, revenue, runtime, movie_status, tagline, vote_average, vote_count) VALUES
+(5,'Four Rooms',4000000,'','It''s Ted the Bellhop''s first night on the job...and the hotel''s very unusual guests are about to place him in some outrageous predicaments. It seems that this evening''s room service is serving up one unbelievable happening after another.',22.876230,'1995-12-09',4300000,98,'Released','Twelve outrageous guests. Four scandalous requests. And one lone bellhop, in his first day on the job, who''s in for the wildest New year''s Eve of his life.',6.50,530),
+(11,'Star Wars',11000000,'http://www.starwars.com/films/star-wars-episode-iv-a-new-hope','Princess Leia is captured and held hostage by the evil Imperial forces in their effort to take over the galactic Empire. Venturesome Luke Skywalker and dashing captain Han Solo team together with the loveable robot duo R2-D2 and C-3PO to rescue the beautiful princess and restore peace and justice in the Empire.',126.393695,'1977-05-25',775398007,121,'Released','A long time ago in a galaxy far, far away...',8.10,6624),
+(12,'Finding Nemo',94000000,'http://movies.disney.com/finding-nemo','Nemo, an adventurous young clownfish, is unexpectedly taken from his Great Barrier Reef home to a dentist''s office aquarium. It''s up to his worrisome father Marlin and a friendly but forgetful fish Dory to bring Nemo home -- meeting vegetarian sharks, surfer dude turtles, hypnotic jellyfish, hungry seagulls, and more along the way.',85.688789,'2003-05-30',940335536,100,'Released','There are 3.7 trillion fish in the ocean, they''re looking for one.',7.60,6122),
+(13,'Forrest Gump',55000000,'','A man with a low IQ has accomplished great things in his life and been present during significant historic events - in each case, far exceeding what anyone imagined he could do. Yet, despite all the things he has attained, his one true love eludes him. ''Forrest Gump'' is the story of a man who rose above his challenges, and who proved that determination, courage, and love are more important than ability.',138.133331,'1994-07-06',677945399,142,'Released','The world will never be the same, once you''ve seen it through the eyes of Forrest Gump.',8.20,7927),
+(14,'American Beauty',15000000,'http://www.dreamworks.com/ab/','Lester Burnham, a depressed suburban father in a mid-life crisis, decides to turn his hectic life around after developing an infatuation with his daughter''s attractive friend.',80.878605,'1999-09-15',356296601,122,'Released','Look closer.',7.90,3313),
+(16,'Dancer in the Dark',12800000,'','Selma, a Czech immigrant on the verge of blindness, struggles to make ends meet for herself and her son, who has inherited the same genetic disorder and will suffer the same fate without an expensive operation. When life gets too difficult, Selma learns to cope through her love of musicals, escaping life''s troubles - even if just for a moment - by dreaming up little numbers to the rhythmic beats of her surroundings.',22.022228,'2000-05-17',40031879,140,'Released','You don''t need eyes to see.',7.60,377),
+(18,'The Fifth Element',90000000,'','In 2257, a taxi driver is unintentionally given the task of saving a young girl who is part of the key that will ensure the survival of humanity.',109.528572,'1997-05-07',263920180,126,'Released','There is no future without it.',7.30,3885),
+(19,'Metropolis',92620000,'','In a futuristic city sharply divided between the working class and the city planners, the son of the city''s mastermind falls in love with a working class prophet who predicts the coming of a savior to mediate their differences.',32.351527,'1927-01-10',650422,153,'Released','There can be no understanding between the hands and the brain unless the heart acts as mediator.',8.00,657),
+(20,'My Life Without Me',0,'http://www.clubcultura.com/clubcine/clubcineastas/isabelcoixet/mividasinmi/index.htm','A Pedro Almodovar production in which a fatally ill mother with only two months to live creates a list of things she wants to do before she dies with out telling her family of her illness.',7.958831,'2003-03-07',9726954,106,'Released','',7.20,77),
+(22,'Pirates of the Caribbean: The Curse of the Black Pearl',140000000,'http://disney.go.com/disneyvideos/liveaction/pirates/main_site/main.html','Jack Sparrow, a freewheeling 17th-century pirate who roams the Caribbean Sea, butts heads with a rival pirate bent on pillaging the village of Port Royal. When the governor''s daughter is kidnapped, Sparrow decides to help the girl''s love save her. But their seafaring mission is hardly simple.',271.972889,'2003-07-09',655011224,143,'Released','Prepare to be blown out of the water.',7.50,6985),
+(24,'Kill Bill: Vol. 1',30000000,'http://www.miramax.com/movie/kill-bill-volume-1/','An assassin is shot at the altar by her ruthless employer, Bill and other members of their assassination circle – but ''The Bride'' lives to plot her vengeance. Setting out for some payback, she makes a death list and hunts down those who wronged her, saving Bill for last.',79.754966,'2003-10-10',180949000,111,'Released','Go for the kill.',7.70,4949),
+(25,'Jarhead',72000000,'','Jarhead is a film about a US Marine Anthony Swofford’s experience in the Gulf War. After putting up with an arduous boot camp, Swafford and his unit are sent to the Persian Gulf where they are earger to fight but are forced to stay back from the action. Meanwhile Swofford gets news of his girlfriend is cheating on him. Desperately he wants to kill someone and finally put his training to use.',32.227223,'2005-11-04',96889998,125,'Released','Welcome to the suck.',6.60,765),
+(28,'Apocalypse Now',31500000,'http://www.apocalypsenow.com','At the height of the Vietnam war, Captain Benjamin Willard is sent on a dangerous mission that, officially, \"does not exist, nor will it ever exist.\" His goal is to locate - and eliminate - a mysterious Green Beret Colonel named Walter Kurtz, who has been leading his personal army on illegal guerrilla missions into enemy territory.',49.973462,'1979-08-15',89460381,153,'Released','This is the end...',8.00,2055),
+(33,'Unforgiven',14000000,'','William Munny is a retired, once-ruthless killer turned gentle widower and hog farmer. To help support his two motherless children, he accepts one last bounty-hunter mission to find the men who brutalized a prostitute. Joined by his former partner and a cocky greenhorn, he takes on a corrupt sheriff.',37.380435,'1992-08-07',159157447,131,'Released','Some legends will never be forgotten. Some wrongs can never be forgiven.',7.70,1113);
+
+
+SELECT * FROM movie;
+
+
+
 #load the necessary libraries
 import pandas as pd
 import sqlalchemy
 
 engine = sqlalchemy.create_engine('mysql+pymysql://root:root@localhost:3306/movies')
 
 df = pd.read_sql_table("movie",engine)
```

