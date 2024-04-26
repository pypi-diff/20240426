# Comparing `tmp/pytgpt_bot-0.0.6.tar.gz` & `tmp/pytgpt_bot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.0.6.tar", last modified: Thu Apr 25 18:07:06 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.0.7.tar", last modified: Fri Apr 26 01:17:19 2024, max compression
```

## Comparing `pytgpt_bot-0.0.6.tar` & `pytgpt_bot-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:07:06.625783 pytgpt_bot-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-25 18:07:06.625783 pytgpt_bot-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:07:06.625783 pytgpt_bot-0.0.6/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:07:06.625783 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:07:06.625783 pytgpt_bot-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:17:19.544592 pytgpt_bot-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 01:17:19.544592 pytgpt_bot-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:17:19.540592 pytgpt_bot-0.0.7/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18621 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:17:19.540592 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 01:17:19.544592 pytgpt_bot-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/setup.py
```

### Comparing `pytgpt_bot-0.0.6/LICENSE` & `pytgpt_bot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.6/PKG-INFO` & `pytgpt_bot-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -87,50 +87,63 @@
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
 ### Commands
 
-- `/help`: This command displays the help information, providing users with a list of available commands and a brief description of what each command does. It's a useful way for users to quickly understand how to interact with the bot.
 
-- `/chat`: Allows users to engage in natural language conversations with the AI. This command initiates a chat session where users can ask questions, make requests, or simply chat with the AI.
+### Usage Information
 
-- `/image`: This command is used to generate images from text descriptions. Users can input a text description, and the bot will attempt to create an image based on that description. This feature can be particularly useful for visualizing ideas or concepts.
+This section provides detailed instructions on how to use the various commands available in the bot.
 
-- `/prodia`: Similar to `/image`, this command also generates images from text descriptions. However, it uses a different provider (Prodia) to create the images. This could offer a different style or interpretation of the text descriptions compared to the default method.
+- **/start**: Displays the help information, offering a comprehensive list of available commands and their functionalities. This command is essential for users to quickly understand how to interact with the bot.
 
-- `/audio`: Converts text to speech. Users can input text, and the bot will generate an audio file that reads out the text. This can be useful for listening to descriptions, instructions, or any text content.
+- **/chat**: Initiate a natural language conversation with the AI. This command allows users to engage in interactive dialogues, ask questions, or make requests.
 
-- `/sintro`: Allows users to set a new text for the chat intro. This can be used to customize the greeting message that users see when they start a new chat session with the bot.
+- **/image**: Generates images from textual descriptions using the default provider. This feature enables users to visualize ideas or concepts through images.
 
-- `/svoice`: Lets users set a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
+- **/prodia**: Generates images from textual descriptions using the Prodia provider. This command offers a unique style or interpretation of the text descriptions compared to the default method.
 
-- `/awesome`: Sets an awesome prompt as the introductory message for the chat. This could be a motivational quote, a fun fact, or any other type of prompt that might inspire or engage users in their interactions with the bot.
+- **/audio**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
 
-- `/history`: Checks the chat history. This command allows users to view the history of their chats with the bot. It can be useful for users who want to review past interactions or find specific information from previous conversations.
+- **/intro**: Sets a new text for the chat intro. This command allows users to customize the chat introductory prompt which serves as a guide in the human-AI engagement.
 
-- `/settings`: Checks the current settings of the bot. This command provides users with an overview of the bot's current configuration, including any custom settings they have applied.
+- **/voice**: Sets a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
 
-- `/reset`: Starts a new chat thread. This command resets the chat history and starts a new conversation thread. It's useful for users who want to start fresh or who want to clear their chat history for privacy reasons.
+- **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
 
-- `/myid`: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for any reason, such as setting up bot admin.
+- **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of them.
+
+- **/history**: Provides users with the ability to view the history of their chats with the bot. This command is useful for reviewing past interactions or finding specific information from previous conversations.
+
+- **/settings**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
+
+- **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
+
+- **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
+
+- `any other text or command>`: An alias for `/chat`, allowing users to continue with text chat.
+
+
+### Administrative Commands
 
-- `/default`: Chat with AI. This command is essentially an alias for `/chat`, allowing users to initiate a chat session with the AI using a different command.
 
 ### Administrative Commands
 
 - `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
 
 - `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
 
-- `/drop`: Clears the entire chat table. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data.
+- `/drop`: Clears the entire chat table and bot logs. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data and current contents of log file.
 
 - `/sql`: Allows running SQL statements against the database. This command provides a way for administrators to directly interact with the bot's database using SQL queries. It's a powerful tool for managing and analyzing the bot's data but should be used with caution to avoid unintended data loss or corruption.
 
+- `/logs`: Checks the logs. This command is used to access the bot's logs, which can provide insights into the bot's activity, errors, and user interactions. It's a valuable tool for monitoring and troubleshooting the bot's performance.
+
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
 
 ## License
 
 `pytgpt-bot` is open-source and available under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code as you see fit.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.6 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.7 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -36,61 +36,61 @@
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the server
 `python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
-Features ### Commands - `/help`: This command displays the help information,
-providing users with a list of available commands and a brief description of
-what each command does. It's a useful way for users to quickly understand how
-to interact with the bot. - `/chat`: Allows users to engage in natural language
-conversations with the AI. This command initiates a chat session where users
-can ask questions, make requests, or simply chat with the AI. - `/image`: This
-command is used to generate images from text descriptions. Users can input a
-text description, and the bot will attempt to create an image based on that
-description. This feature can be particularly useful for visualizing ideas or
-concepts. - `/prodia`: Similar to `/image`, this command also generates images
-from text descriptions. However, it uses a different provider (Prodia) to
-create the images. This could offer a different style or interpretation of the
-text descriptions compared to the default method. - `/audio`: Converts text to
-speech. Users can input text, and the bot will generate an audio file that
-reads out the text. This can be useful for listening to descriptions,
-instructions, or any text content. - `/sintro`: Allows users to set a new text
-for the chat intro. This can be used to customize the greeting message that
-users see when they start a new chat session with the bot. - `/svoice`: Lets
-users set a new voice for speech synthesis. This command enables users to
-choose from different voices for the AI to use when generating audio from text.
-- `/awesome`: Sets an awesome prompt as the introductory message for the chat.
-This could be a motivational quote, a fun fact, or any other type of prompt
-that might inspire or engage users in their interactions with the bot. - `/
-history`: Checks the chat history. This command allows users to view the
-history of their chats with the bot. It can be useful for users who want to
-review past interactions or find specific information from previous
-conversations. - `/settings`: Checks the current settings of the bot. This
-command provides users with an overview of the bot's current configuration,
-including any custom settings they have applied. - `/reset`: Starts a new chat
-thread. This command resets the chat history and starts a new conversation
-thread. It's useful for users who want to start fresh or who want to clear
-their chat history for privacy reasons. - `/myid`: Echoes the user's Telegram
-ID. This command is useful for users who need to know their Telegram ID for any
-reason, such as setting up bot admin. - `/default`: Chat with AI. This command
-is essentially an alias for `/chat`, allowing users to initiate a chat session
-with the AI using a different command. ### Administrative Commands - `/clear`:
-Clears all chats. This command is used to remove all chat data from the bot's
-database. It's a powerful command that should be used with caution, as it will
-delete all chat history. - `/total`: Shows the total number of chats available.
-This command provides an overview of the current chat data stored in the bot's
-database, helping administrators understand the volume of interactions the bot
-has had. - `/drop`: Clears the entire chat table. Similar to `/clear`, this
-command removes all data from the chat table in the database. It's a more
-drastic measure than `/clear`, as it completely wipes out all chat data. - `/
-sql`: Allows running SQL statements against the database. This command provides
-a way for administrators to directly interact with the bot's database using SQL
-queries. It's a powerful tool for managing and analyzing the bot's data but
-should be used with caution to avoid unintended data loss or corruption. ##
+Features ### Commands ### Usage Information This section provides detailed
+instructions on how to use the various commands available in the bot. - **/
+start**: Displays the help information, offering a comprehensive list of
+available commands and their functionalities. This command is essential for
+users to quickly understand how to interact with the bot. - **/chat**: Initiate
+a natural language conversation with the AI. This command allows users to
+engage in interactive dialogues, ask questions, or make requests. - **/image**:
+Generates images from textual descriptions using the default provider. This
+feature enables users to visualize ideas or concepts through images. - **/
+prodia**: Generates images from textual descriptions using the Prodia provider.
+This command offers a unique style or interpretation of the text descriptions
+compared to the default method. - **/audio**: Converts text to speech,
+providing users with the ability to listen to descriptions, instructions, or
+any text content read out by the AI. - **/intro**: Sets a new text for the chat
+intro. This command allows users to customize the chat introductory prompt
+which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
+voice for speech synthesis. This command enables users to choose from different
+voices for the AI to use when generating audio from text. - **/provider**: Sets
+a new chat provider. This command allows users to switch between different
+providers for various functionalities, such as `phind`, `llama2`, `koboldai`
+etc. - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of
+them. - **/history**: Provides users with the ability to view the history of
+their chats with the bot. This command is useful for reviewing past
+interactions or finding specific information from previous conversations. - **/
+settings**: Offers an overview of the bot's current configuration, including
+any custom settings applied by the user. - **/reset**: Resets the chat history
+and starts a new conversation thread. This command is useful for users who wish
+to start fresh or clear their chat history for privacy reasons. - **/myid**:
+Echoes the user's Telegram ID. This command is useful for users who need to
+know their Telegram ID for various purposes, such as setting up bot admin. -
+`any other text or command>`: An alias for `/chat`, allowing users to continue
+with text chat. ### Administrative Commands ### Administrative Commands - `/
+clear`: Clears all chats. This command is used to remove all chat data from the
+bot's database. It's a powerful command that should be used with caution, as it
+will delete all chat history. - `/total`: Shows the total number of chats
+available. This command provides an overview of the current chat data stored in
+the bot's database, helping administrators understand the volume of
+interactions the bot has had. - `/drop`: Clears the entire chat table and bot
+logs. Similar to `/clear`, this command removes all data from the chat table in
+the database. It's a more drastic measure than `/clear`, as it completely wipes
+out all chat data and current contents of log file. - `/sql`: Allows running
+SQL statements against the database. This command provides a way for
+administrators to directly interact with the bot's database using SQL queries.
+It's a powerful tool for managing and analyzing the bot's data but should be
+used with caution to avoid unintended data loss or corruption. - `/logs`:
+Checks the logs. This command is used to access the bot's logs, which can
+provide insights into the bot's activity, errors, and user interactions. It's a
+valuable tool for monitoring and troubleshooting the bot's performance. ##
 Support and Feedback If you have any questions, feedback, or suggestions for
 `pytgpt`, please feel free to reach out. Your input is valuable in helping us
 improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
 source and available under the [MIT License](LICENSE). Feel free to use,
 modify, and distribute the code as you see fit. --- Thank you for using
 `pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.0.6/README.md` & `pytgpt_bot-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -49,50 +49,63 @@
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
 ### Commands
 
-- `/help`: This command displays the help information, providing users with a list of available commands and a brief description of what each command does. It's a useful way for users to quickly understand how to interact with the bot.
 
-- `/chat`: Allows users to engage in natural language conversations with the AI. This command initiates a chat session where users can ask questions, make requests, or simply chat with the AI.
+### Usage Information
 
-- `/image`: This command is used to generate images from text descriptions. Users can input a text description, and the bot will attempt to create an image based on that description. This feature can be particularly useful for visualizing ideas or concepts.
+This section provides detailed instructions on how to use the various commands available in the bot.
 
-- `/prodia`: Similar to `/image`, this command also generates images from text descriptions. However, it uses a different provider (Prodia) to create the images. This could offer a different style or interpretation of the text descriptions compared to the default method.
+- **/start**: Displays the help information, offering a comprehensive list of available commands and their functionalities. This command is essential for users to quickly understand how to interact with the bot.
 
-- `/audio`: Converts text to speech. Users can input text, and the bot will generate an audio file that reads out the text. This can be useful for listening to descriptions, instructions, or any text content.
+- **/chat**: Initiate a natural language conversation with the AI. This command allows users to engage in interactive dialogues, ask questions, or make requests.
 
-- `/sintro`: Allows users to set a new text for the chat intro. This can be used to customize the greeting message that users see when they start a new chat session with the bot.
+- **/image**: Generates images from textual descriptions using the default provider. This feature enables users to visualize ideas or concepts through images.
 
-- `/svoice`: Lets users set a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
+- **/prodia**: Generates images from textual descriptions using the Prodia provider. This command offers a unique style or interpretation of the text descriptions compared to the default method.
 
-- `/awesome`: Sets an awesome prompt as the introductory message for the chat. This could be a motivational quote, a fun fact, or any other type of prompt that might inspire or engage users in their interactions with the bot.
+- **/audio**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
 
-- `/history`: Checks the chat history. This command allows users to view the history of their chats with the bot. It can be useful for users who want to review past interactions or find specific information from previous conversations.
+- **/intro**: Sets a new text for the chat intro. This command allows users to customize the chat introductory prompt which serves as a guide in the human-AI engagement.
 
-- `/settings`: Checks the current settings of the bot. This command provides users with an overview of the bot's current configuration, including any custom settings they have applied.
+- **/voice**: Sets a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
 
-- `/reset`: Starts a new chat thread. This command resets the chat history and starts a new conversation thread. It's useful for users who want to start fresh or who want to clear their chat history for privacy reasons.
+- **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
 
-- `/myid`: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for any reason, such as setting up bot admin.
+- **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of them.
+
+- **/history**: Provides users with the ability to view the history of their chats with the bot. This command is useful for reviewing past interactions or finding specific information from previous conversations.
+
+- **/settings**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
+
+- **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
+
+- **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
+
+- `any other text or command>`: An alias for `/chat`, allowing users to continue with text chat.
+
+
+### Administrative Commands
 
-- `/default`: Chat with AI. This command is essentially an alias for `/chat`, allowing users to initiate a chat session with the AI using a different command.
 
 ### Administrative Commands
 
 - `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
 
 - `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
 
-- `/drop`: Clears the entire chat table. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data.
+- `/drop`: Clears the entire chat table and bot logs. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data and current contents of log file.
 
 - `/sql`: Allows running SQL statements against the database. This command provides a way for administrators to directly interact with the bot's database using SQL queries. It's a powerful tool for managing and analyzing the bot's data but should be used with caution to avoid unintended data loss or corruption.
 
+- `/logs`: Checks the logs. This command is used to access the bot's logs, which can provide insights into the bot's activity, errors, and user interactions. It's a valuable tool for monitoring and troubleshooting the bot's performance.
+
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
 
 ## License
 
 `pytgpt-bot` is open-source and available under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code as you see fit.
```

#### html2text {}

```diff
@@ -12,61 +12,61 @@
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the server
 `python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
-Features ### Commands - `/help`: This command displays the help information,
-providing users with a list of available commands and a brief description of
-what each command does. It's a useful way for users to quickly understand how
-to interact with the bot. - `/chat`: Allows users to engage in natural language
-conversations with the AI. This command initiates a chat session where users
-can ask questions, make requests, or simply chat with the AI. - `/image`: This
-command is used to generate images from text descriptions. Users can input a
-text description, and the bot will attempt to create an image based on that
-description. This feature can be particularly useful for visualizing ideas or
-concepts. - `/prodia`: Similar to `/image`, this command also generates images
-from text descriptions. However, it uses a different provider (Prodia) to
-create the images. This could offer a different style or interpretation of the
-text descriptions compared to the default method. - `/audio`: Converts text to
-speech. Users can input text, and the bot will generate an audio file that
-reads out the text. This can be useful for listening to descriptions,
-instructions, or any text content. - `/sintro`: Allows users to set a new text
-for the chat intro. This can be used to customize the greeting message that
-users see when they start a new chat session with the bot. - `/svoice`: Lets
-users set a new voice for speech synthesis. This command enables users to
-choose from different voices for the AI to use when generating audio from text.
-- `/awesome`: Sets an awesome prompt as the introductory message for the chat.
-This could be a motivational quote, a fun fact, or any other type of prompt
-that might inspire or engage users in their interactions with the bot. - `/
-history`: Checks the chat history. This command allows users to view the
-history of their chats with the bot. It can be useful for users who want to
-review past interactions or find specific information from previous
-conversations. - `/settings`: Checks the current settings of the bot. This
-command provides users with an overview of the bot's current configuration,
-including any custom settings they have applied. - `/reset`: Starts a new chat
-thread. This command resets the chat history and starts a new conversation
-thread. It's useful for users who want to start fresh or who want to clear
-their chat history for privacy reasons. - `/myid`: Echoes the user's Telegram
-ID. This command is useful for users who need to know their Telegram ID for any
-reason, such as setting up bot admin. - `/default`: Chat with AI. This command
-is essentially an alias for `/chat`, allowing users to initiate a chat session
-with the AI using a different command. ### Administrative Commands - `/clear`:
-Clears all chats. This command is used to remove all chat data from the bot's
-database. It's a powerful command that should be used with caution, as it will
-delete all chat history. - `/total`: Shows the total number of chats available.
-This command provides an overview of the current chat data stored in the bot's
-database, helping administrators understand the volume of interactions the bot
-has had. - `/drop`: Clears the entire chat table. Similar to `/clear`, this
-command removes all data from the chat table in the database. It's a more
-drastic measure than `/clear`, as it completely wipes out all chat data. - `/
-sql`: Allows running SQL statements against the database. This command provides
-a way for administrators to directly interact with the bot's database using SQL
-queries. It's a powerful tool for managing and analyzing the bot's data but
-should be used with caution to avoid unintended data loss or corruption. ##
+Features ### Commands ### Usage Information This section provides detailed
+instructions on how to use the various commands available in the bot. - **/
+start**: Displays the help information, offering a comprehensive list of
+available commands and their functionalities. This command is essential for
+users to quickly understand how to interact with the bot. - **/chat**: Initiate
+a natural language conversation with the AI. This command allows users to
+engage in interactive dialogues, ask questions, or make requests. - **/image**:
+Generates images from textual descriptions using the default provider. This
+feature enables users to visualize ideas or concepts through images. - **/
+prodia**: Generates images from textual descriptions using the Prodia provider.
+This command offers a unique style or interpretation of the text descriptions
+compared to the default method. - **/audio**: Converts text to speech,
+providing users with the ability to listen to descriptions, instructions, or
+any text content read out by the AI. - **/intro**: Sets a new text for the chat
+intro. This command allows users to customize the chat introductory prompt
+which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
+voice for speech synthesis. This command enables users to choose from different
+voices for the AI to use when generating audio from text. - **/provider**: Sets
+a new chat provider. This command allows users to switch between different
+providers for various functionalities, such as `phind`, `llama2`, `koboldai`
+etc. - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of
+them. - **/history**: Provides users with the ability to view the history of
+their chats with the bot. This command is useful for reviewing past
+interactions or finding specific information from previous conversations. - **/
+settings**: Offers an overview of the bot's current configuration, including
+any custom settings applied by the user. - **/reset**: Resets the chat history
+and starts a new conversation thread. This command is useful for users who wish
+to start fresh or clear their chat history for privacy reasons. - **/myid**:
+Echoes the user's Telegram ID. This command is useful for users who need to
+know their Telegram ID for various purposes, such as setting up bot admin. -
+`any other text or command>`: An alias for `/chat`, allowing users to continue
+with text chat. ### Administrative Commands ### Administrative Commands - `/
+clear`: Clears all chats. This command is used to remove all chat data from the
+bot's database. It's a powerful command that should be used with caution, as it
+will delete all chat history. - `/total`: Shows the total number of chats
+available. This command provides an overview of the current chat data stored in
+the bot's database, helping administrators understand the volume of
+interactions the bot has had. - `/drop`: Clears the entire chat table and bot
+logs. Similar to `/clear`, this command removes all data from the chat table in
+the database. It's a more drastic measure than `/clear`, as it completely wipes
+out all chat data and current contents of log file. - `/sql`: Allows running
+SQL statements against the database. This command provides a way for
+administrators to directly interact with the bot's database using SQL queries.
+It's a powerful tool for managing and analyzing the bot's data but should be
+used with caution to avoid unintended data loss or corruption. - `/logs`:
+Checks the logs. This command is used to access the bot's logs, which can
+provide insights into the bot's activity, errors, and user interactions. It's a
+valuable tool for monitoring and troubleshooting the bot's performance. ##
 Support and Feedback If you have any questions, feedback, or suggestions for
 `pytgpt`, please feel free to reach out. Your input is valuable in helping us
 improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
 source and available under the [MIT License](LICENSE). Feel free to use,
 modify, and distribute the code as you see fit. --- Thank you for using
 `pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.0.6/pytgpt_bot/cli.py` & `pytgpt_bot-0.0.7/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.6/pytgpt_bot/db.py` & `pytgpt_bot-0.0.7/pytgpt_bot/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,17 @@
         """Creates database"""
         conn = sqlite3.connect(path_to_db)
         conn.execute(
             f"""
         CREATE TABLE IF NOT EXISTS Chat(
             Id INTEGER PRIMARY KEY,
             Intro TEXT DEFAULT "{Conversation.intro}",
-            History TEXT DEFAULT "",
-            Voice TEXT DEFAULT "Brian"
+            History TEXT DEFAULT "" NOT NULL,
+            Voice TEXT DEFAULT "Brian" NOT NULL,
+            Provider TEXT DEFAULT "auto" NOT NULL
             );
         """
         )
         conn.commit()
 
     @staticmethod
     @exception_handler
@@ -149,32 +150,37 @@
     @property
     def record(self) -> typing.Dict[str, typing.Union[int, str]]:
         """User data
 
         Returns:
             typing.Dict[str, typing.Union[int, str]]: Records
         """
-        id, intro, history, voice = Chat.read(id=self.id, fetchone=True)
-        return dict(id=id, intro=intro, history=history, voice=voice)
+        id, intro, history, voice, provider = Chat.read(id=self.id, fetchone=True)
+        return dict(id=id, intro=intro, history=history, voice=voice, provider=provider)
 
     @property
     def chat_history(self) -> typing.Union[str, None]:
         """User's chat history"""
         return self.record.get("history")
 
     @property
     def chat_intro(self) -> str:
         """User's chat intro"""
         return self.record.get("intro")
 
     @property
-    def chat_voice(self) -> typing.Union[str, None]:
+    def chat_voice(self) -> str:
         """User's speech voice"""
         return self.record.get("voice")
 
+    @property
+    def chat_provider(self) -> str:
+        """User's text chat provider"""
+        return self.record.get("provider")
+
     def update_history(self, data: str):
         """Update chat history
 
         Args:
             data (str): New history
         """
         Chat.update(
@@ -203,14 +209,26 @@
         """
         Chat.update(
             self.id,
             field="voice",
             data=data,
         )
 
+    def update_provider(self, data: str):
+        """Update text provider
+
+        Args:
+            data (str): New provider.
+        """
+        Chat.update(
+            self.id,
+            field="provider",
+            data=data,
+        )
+
     def delete(self):
         """Delete current user account"""
         Chat.delete(self.id)
 
 
 # import os
 # os.remove(path_to_db)
```

### Comparing `pytgpt_bot-0.0.6/pytgpt_bot/main.py` & `pytgpt_bot-0.0.7/pytgpt_bot/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,53 @@
 import telebot
-import pytgpt.auto as text_generator
 import pytgpt.imager as image_generator
 from pytgpt.utils import Audio as audio_generator
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
 from functools import wraps
 import logging
 
-from .config import bot_token, max_tokens, timeout, voice, loglevel, logfile, admin_id
+from pytgpt.opengpt import OPENGPT
+from pytgpt.koboldai import KOBOLDAI
+from pytgpt.phind import PHIND
+from pytgpt.llama2 import LLAMA2
+from pytgpt.blackboxai import BLACKBOXAI
+from pytgpt.perplexity import PERPLEXITY
+from pytgpt.yepchat import YEPCHAT
+from pytgpt.auto import AUTO
+
+from .config import (
+    bot_token,
+    max_tokens,
+    timeout,
+    loglevel,
+    logfile,
+    admin_id,
+    provider,
+)
 from .db import User, Chat
+from . import __version__
+
+provider_map: dict[str, object] = {
+    "opengpt": OPENGPT,
+    "koboldai": KOBOLDAI,
+    "phind": PHIND,
+    "llama2": LLAMA2,
+    "blackboxai": BLACKBOXAI,
+    "perplexity": PERPLEXITY,
+    "yepchat": YEPCHAT,
+    "auto": AUTO,
+}
+
+chosen_provider: str = provider_map.get(provider)
+provider_keys: list = list(provider_map.keys())
+
+assert (
+    chosen_provider
+), f"Provider '{provider}' is not one of {', '.join(provider_keys)}"
 
 log_params = dict(
     format="%(asctime)s : %(levelname)s - %(message)s",
     datefmt="%d-%b-%Y %H:%M:%S",
     level=loglevel,
 )
 
@@ -29,16 +64,17 @@
 bot.remove_webhook()
 
 logging.info(f"Bot started sucessfully. Admin ID - [{admin_id}]")
 
 admin_commands = """
     /clear : Clear all chats.
     /total : Total chats available.
-    /drop : Clear entire chat table.
+    /drop : Clear entire chat table and bot logs.
     /sql : Run sql statements against database.
+    /logs : View bot logs.
 """
 
 
 def handler_formatter(text: bool = False, admin: bool = False):
     """Handles common message handler verification and execptions
 
     Args:
@@ -51,144 +87,228 @@
         @wraps(func)
         def decorator(message: telebot.types.Message):
             try:
                 logging.info(
                     f"Serving user [{message.from_user.id}] ({message.from_user.full_name}) - Function [{func.__name__}]"
                 )
                 if admin and not User(message.from_user.id).is_admin:
-                    return bot.reply_to(message, "Action restricted to admins only!")
+                    return bot.reply_to(
+                        message,
+                        "Action restricted to admins only❗️",
+                        reply_markup=make_delete_markup(message),
+                    )
 
                 if message.text and message.text.startswith("/"):
                     message.text = " ".join(message.text.split(" ")[1:])
 
                 if text and not message.text:
-                    return bot.reply_to(message, "Text is required.")
+                    return bot.reply_to(
+                        message,
+                        "Text is required❗️❗️.",
+                        reply_markup=make_delete_markup(message),
+                    )
 
                 return func(message)
             except Exception as e:
                 logging.error(f"Error on function - {func.__name__} - {e}")
                 logging.exception(e)
-                return bot.reply_to(
-                    message, text="An error occured and could't complete that request."
+                bot.reply_to(
+                    message,
+                    text="😔 An error occured and I could't complete that request ❗️❗️❗️",
+                    reply_markup=make_delete_markup(message),
                 )
 
         return decorator
 
     return main
 
 
-def send_long_text(message: telebot.types.Message, text: str):
+def make_delete_markup(
+    message: telebot.types.Message,
+) -> telebot.types.InlineKeyboardMarkup:
+    """Creates delete markup
+
+    Args:
+        message (telebot.types.Message):
+    """
+    markup = telebot.types.InlineKeyboardMarkup(row_width=1)
+    callback_button = telebot.types.InlineKeyboardButton(
+        text="🗑️", callback_data=f"delete:{message.chat.id}:{message.id}"
+    )
+    markup.add(callback_button)
+    return markup
+
+
+def send_and_add_delete_button(
+    message: telebot.types.Message, text: str, as_reply: bool = False
+):
+    """Add send text and add delete inlineKeyboard item
+
+    Args:
+        message (telebot.types.Message):
+        text (str): Tag
+        as_reply (bool): Respond as a reply_to. Defaults to False.
+
+    Returns:
+        _type_: _description_
+    """
+    markup = make_delete_markup(message)
+    return (
+        bot.reply_to(message, text=text, reply_markup=markup)
+        if as_reply
+        else bot.send_message(message.chat.id, text, reply_markup=markup)
+    )
+
+
+def send_long_text(message: telebot.types.Message, text: str, add_delete: bool = False):
     """Send texts longer than 4096 long
 
     Args:
         message (telebot.types.Message): Message object.
         text (str): Text to be sent.
+        add_delete (bool). Add delete button. Defaults to False.
     """
     max_length = 4096
+    take_action = send_and_add_delete_button if add_delete else bot.send_message
     if len(text) <= max_length:
-        bot.send_message(message.chat.id, text)
+        # bot.send_message(message.chat.id, text)
+        take_action(message if add_delete else message.chat.id, text)
     else:
         parts = [text[i : i + max_length] for i in range(0, len(text), max_length)]
         for part in parts:
-            bot.send_message(message.chat.id, part)
+            take_action(message if add_delete else message.chat.id, part)
 
 
 @bot.message_handler(commands=["help", "start"])
 @handler_formatter()
 def home(message: telebot.types.Message):
     """
-    Welcome to [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot).
-    /help : Show this help info.
+    Welcome to [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot). Freely interact with multiple LLM providers.
+    /start : Show this help info.
     /chat : Chat with AI.
-    /imager : Generate image from text. (default)
+    /image : Generate image from text. (default)
     /prodia : Generate image from text. (Prodia)
     /audio : Generate audio from text.
-    /sintro : Set new text for chat intro.
-    /svoice : Set new voice for speech synthesis.
+    /intro : Set new text for chat intro.
+    /voice : Set new voice for speech synthesis.
+    /provider : Set new chat provider.
     /awesome : Set awesome prompt as intro.
     /history : Check chat history.
     /settings : Check current settings.
     /reset : Start new chat thread.
     /myid : Echo your Telegram ID.
     /default : Chat with AI.
     """
 
     return bot.send_message(
         message.chat.id,
         text=(
             home.__doc__ + admin_commands if User(message.from_user.id).is_admin else ""
         ),
+        reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["myid"])
 @handler_formatter()
 def echo_user_id(message: telebot.types.Message):
     return bot.reply_to(
         message,
         f"Greetings {message.from_user.first_name}. Your Telegram ID is {message.from_user.id}.",
+        reply_markup=make_delete_markup(message),
     )
 
 
-@bot.message_handler(commands=["sintro"])
+@bot.message_handler(commands=["intro"])
 @handler_formatter(text=True)
 def set_chat_intro(message: telebot.types.Message):
     """Set new value for chat intro"""
     intro = AwesomePrompts().get_act(message.text) or message.text
     if not len(intro) > 10:
         return bot.reply_to(
-            message, "The chat introduction must be at least 10 characters long."
+            message,
+            "The chat introduction must be at least 10 characters long.",
+            reply_markup=make_delete_markup(message),
         )
     user = User(message.from_user.id)
     user.update_intro(intro)
-    bot.reply_to(message, "New intro set successfully.")
+    return bot.reply_to(
+        message, "New intro set successfully.", reply_markup=make_delete_markup(message)
+    )
 
 
-@bot.message_handler(commands=["svoice"])
+@bot.message_handler(commands=["voice"])
 @handler_formatter(text=False)
-def set_new_chat_intro(message: telebot.types.Message):
+def set_new_speech_voice(message: telebot.types.Message):
     """Set new voice for speech synthesis"""
     user_id: str = message.from_user.id
     markup = telebot.types.InlineKeyboardMarkup(row_width=4)
     make_item = lambda voice: telebot.types.InlineKeyboardButton(
         voice, callback_data=f"{voice}:{user_id}"
     )
     markup.add(*map(make_item, audio_generator.all_voices))
-
+    bot.delete_message(message.chat.id, message.id)
     return bot.send_message(message.chat.id, "Choose a voice:", reply_markup=markup)
 
 
 @bot.callback_query_handler(
     func=lambda call: call.data.split(":")[0] in audio_generator.all_voices
 )
-def set_new_chat_intro_callback(call: telebot.types.CallbackQuery):
+def set_new_speech_voice_callback(call: telebot.types.CallbackQuery):
     """Set new voice for speech synthesis callback handler"""
     bot.delete_message(call.message.chat.id, call.message.id)
     voice, user_id = call.data.split(":")
     message = call.message
-    if not voice in audio_generator.all_voices:
-        return bot.reply_to(
-            message,
-            f"Voice '{voice}' is not one of : `({', '.join(audio_generator.all_voices)})`",
-        )
+    markup = make_delete_markup(call.message)
     user = User(int(user_id))
     user.update_voice(voice)
-    return bot.send_message(message.chat.id, f"New voice set : `{voice}`")
+    return bot.send_message(
+        message.chat.id, f"New voice set : `{voice}`", reply_markup=markup
+    )
+
+
+@bot.message_handler(commands=["provider"])
+@handler_formatter(text=False)
+def set_new_text_provider(message: telebot.types.Message):
+    """Set new text provider"""
+    user_id: str = message.from_user.id
+    markup = telebot.types.InlineKeyboardMarkup(row_width=2)
+    make_item = lambda provider: telebot.types.InlineKeyboardButton(
+        provider, callback_data=f"{provider}:{user_id}"
+    )
+    markup.add(*map(make_item, provider_keys))
+    bot.delete_message(message.chat.id, message.id)
+    return bot.send_message(message.chat.id, "Choose a provider:", reply_markup=markup)
+
+
+@bot.callback_query_handler(func=lambda call: call.data.split(":")[0] in provider_keys)
+def set_new_text_provider_callback(call: telebot.types.CallbackQuery):
+    """Set new text provider callback handler"""
+    bot.delete_message(call.message.chat.id, call.message.id)
+    provider, user_id = call.data.split(":")
+    message = call.message
+    markup = make_delete_markup(call.message)
+    user = User(int(user_id))
+    user.update_provider(provider)
+    return bot.send_message(
+        message.chat.id, f"New text provider set : `{provider}`", reply_markup=markup
+    )
 
 
 @bot.message_handler(commands=["awesome"])
 @handler_formatter(text=False)
 def set_awesome_prompt_as_chat_intro(message: telebot.types.Message):
     """Set awesome prompt as intro"""
     user_id: str = message.from_user.id
     markup = telebot.types.InlineKeyboardMarkup(row_width=4)
     make_item = lambda awesome: telebot.types.InlineKeyboardButton(
         awesome, callback_data=f"{awesome}:{user_id}"
     )
     markup.add(*map(make_item, awesome_prompts_keys))
+    bot.delete_message(message.chat.id, message.id)
     return bot.send_message(message.chat.id, "Choose awesome:", reply_markup=markup)
 
 
 @bot.callback_query_handler(
     func=lambda call: call.data.split(":")[0] in awesome_prompts_keys
 )
 def set_awesome_prompt_as_chat_intro_callback_handler(
@@ -201,121 +321,148 @@
     user.update_intro(awesome_prompts.get(awesome_prompt))
     return bot.send_message(
         call.message.chat.id,
         f"""New awesome-intro set:
 ```
 {awesome_prompts.get(awesome_prompt)}
 ```.""",
+        reply_markup=make_delete_markup(call.message),
     )
 
 
 @bot.message_handler(commands=["settings"])
 @handler_formatter()
 def check_current_settings(message: telebot.types.Message):
     """Check current user settings"""
-    user = User(message.from_user.id)
+    user_record: dict = User(message.from_user.id).record
     current_user_settings = f"""
-    **Chat Length** : `{len(user.chat_history)}`
-    **Speech Voice** : `{user.chat_voice}`
-    **Chat Intro** : `{user.chat_intro}`
+    **Chat Length** : `{len(user_record.get('history'))}`
+    **Speech Voice** : `{user_record.get('voice')}`
+    **Chat provider** : {user_record.get('provider')}
+    **Chat Intro** : `{user_record.get('intro')}`
     """
-    return bot.reply_to(message, current_user_settings)
+    return bot.reply_to(
+        message, current_user_settings, reply_markup=make_delete_markup(message)
+    )
 
 
 @bot.message_handler(commands=["history"])
 @handler_formatter()
 def check_chat_history(message: telebot.types.Message):
     user = User(message.from_user.id)
-    return send_long_text(message, user.chat_history or "Your chat history is empty.")
+    return send_long_text(
+        message, user.chat_history or "Your chat history is empty ❗️", add_delete=True
+    )
 
 
 @bot.message_handler(commands=["image", "img"])
 @handler_formatter(text=True)
 def text_to_image_default(message: telebot.types.Message):
     """Generate image using `image`"""
     generator_obj = image_generator.Imager(
-        timeout=30,
+        timeout=timeout,
     )
     return bot.send_photo(
         message.chat.id,
         photo=generator_obj.generate(
             message.text,
         )[0],
         caption=message.text,
+        reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["prodia", "prod"])
 @handler_formatter(text=True)
 def text_to_image_prodia(message: telebot.types.Message):
     """Generate image using `prodia`"""
     generator_obj = image_generator.Prodia(timeout=timeout)
     return bot.send_photo(
         message.chat.id,
         photo=generator_obj.generate(message.text)[0],
         caption=message.text,
+        reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["audio", "aud"])
 @handler_formatter(text=True)
 def text_to_audio(message: telebot.types.Message):
     """Convert text to audio"""
     audio_chunk = audio_generator.text_to_audio(
         message=message.text,
         voice=User(message.chat.id).chat_voice,
         timeout=timeout,
     )
-    return bot.send_audio(message.chat.id, audio=audio_chunk, caption=message.text)
+    return bot.send_audio(
+        message.chat.id,
+        audio=audio_chunk,
+        caption=message.text,
+        reply_markup=make_delete_markup(message),
+    )
 
 
 @bot.message_handler(commands=["reset"])
 @handler_formatter()
 def reset_chat(message: telebot.types.Message):
     """Reset current chat thread"""
     user = User(message.from_user.id)
     user.delete()
     return bot.reply_to(
-        message,
-        "New chat instance created.",
+        message, "New chat instance created.", reply_markup=make_delete_markup(message)
     )
 
 
 @bot.message_handler(commands=["clear", "clear_chats"])
 @handler_formatter(admin=True)
 def clear_chats(message: telebot.types.Message):
     """Delete all chat entries"""
     Chat.query("DELETE FROM Chat")
     logging.warning(
         f"Clearing Chats - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
-    return bot.reply_to(message, "Chats cleared successfully.")
+    return bot.reply_to(
+        message, "Chats cleared successfully.", reply_markup=make_delete_markup(message)
+    )
 
 
 @bot.message_handler(commands=["total", "total_chats"])
 @handler_formatter(admin=True)
 def total_chats_query(message: telebot.types.Message):
     """Query total chats"""
     total_chats = Chat.query("SELECT COUNT(id) FROM Chat")[0][0]
     logging.warning(
         f"Total Chats query - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
-    return bot.reply_to(message, f"Total Chats **{total_chats}**")
+    return bot.reply_to(
+        message,
+        f"Total Chats **{total_chats}**",
+        reply_markup=make_delete_markup(message),
+    )
 
 
 @bot.message_handler(commands=["drop", "drop_chats"])
 @handler_formatter(admin=True)
 def total_chats_table(message: telebot.types.Message):
     """Drop chat table and create new"""
+    if logfile:
+        with open(logfile, "w") as fh:
+            fh.write(
+                f"ADMIN CLEARED LOGS & DROPPED CHAT TABLE [{message.from_user.id}] - ({message.from_user.full_name})\n"
+            )
     logging.warning(
         f"Dropping Chat table and reinitialize - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     Chat.query("DROP TABLE CHAT")
     Chat.initialize()
-    return bot.reply_to(message, f"Chat table dropped and new one created.")
+    return bot.reply_to(
+        message,
+        f"Chat table dropped and new one created.",
+        reply_markup=make_delete_markup(message),
+    )
 
 
 @bot.message_handler(commands=["sql"])
 @handler_formatter(admin=True)
 def run_sql_statement(message: telebot.types.Message):
     """Run sql statements against database"""
     logging.warning(
@@ -328,21 +475,32 @@
         ```
         """
 
     except Exception as e:
         response = f"ERROR : {e.args[1] if e.args and len(e.args)>1 else e}"
 
     finally:
-        return send_long_text(message, response)
+        return send_long_text(message, response, add_delete=True)
 
 
-@bot.message_handler(content_types=["text"])
+@bot.message_handler(commands=["logs"])
+@handler_formatter(admin=True)
+def check_current_settings(message: telebot.types.Message):
+    """View bot logs"""
+    if not logfile:
+        return bot.reply_to(message, "Logfile not specified!")
+    with open(logfile, encoding="utf-8") as fh:
+        contents: str = fh.read()
+    return send_long_text(message, contents, add_delete=True)
+
+
+@bot.message_handler(content_types=["chat"])
 @handler_formatter(text=True)
 def text_chat(message: telebot.types.Message):
-    """Text generation"""
+    """Text generation - provider of choice"""
     user = User(message.from_user.id)
     chat_record = user.record
     conversation = Conversation(max_tokens=max_tokens)
     conversation.chat_history = chat_record.get("history") or ""
     conversation_prompt = conversation.gen_complete_prompt(
         message.text, intro=chat_record.get("intro")
     )
@@ -353,10 +511,49 @@
     conversation.update_chat_history(
         prompt=message.text, response=ai_response, force=True
     )
     user.update_history(conversation.chat_history)
     return send_long_text(message, ai_response)
 
 
+@bot.message_handler(content_types=["text"])
+@handler_formatter(text=True)
+def text_chat(message: telebot.types.Message):
+    """Text generation"""
+    user = User(message.from_user.id)
+    chat_record = user.record
+    conversation = Conversation(max_tokens=max_tokens)
+    conversation.chat_history = chat_record.get("history")
+    user_provider = provider_map.get(chat_record.get("provider"))
+    conversation_prompt = conversation.gen_complete_prompt(
+        message.text, intro=chat_record.get("intro")
+    )
+    bot.send_chat_action(message.chat.id, "typing")
+    ai_response = user_provider(is_conversation=False, timeout=timeout).chat(
+        conversation_prompt
+    )
+    conversation.update_chat_history(
+        prompt=message.text, response=ai_response, force=True
+    )
+    user.update_history(conversation.chat_history)
+    return send_long_text(message, ai_response)
+
+
 @bot.message_handler(func=lambda val: True)
 def any_other_action(message):
-    return bot.reply_to(message, home.__doc__)
+    return bot.reply_to(message, home.__doc__, reply_markup=make_delete_markup(message))
+
+
+@bot.callback_query_handler(func=lambda call: call.data.startswith("delete:"))
+def delete_callback_handler(
+    call: telebot.types.CallbackQuery,
+):
+    """Delete callback handler"""
+    action, trigger_chat_id, trigger_message_id = call.data.split(":")
+    try:
+        bot.delete_message(trigger_chat_id, trigger_message_id)
+    except:
+        pass
+    try:
+        bot.delete_message(call.message.chat.id, call.message.id)
+    except:
+        pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytgpt_bot-0.0.6/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.0.7/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -87,50 +87,63 @@
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
 ### Commands
 
-- `/help`: This command displays the help information, providing users with a list of available commands and a brief description of what each command does. It's a useful way for users to quickly understand how to interact with the bot.
 
-- `/chat`: Allows users to engage in natural language conversations with the AI. This command initiates a chat session where users can ask questions, make requests, or simply chat with the AI.
+### Usage Information
 
-- `/image`: This command is used to generate images from text descriptions. Users can input a text description, and the bot will attempt to create an image based on that description. This feature can be particularly useful for visualizing ideas or concepts.
+This section provides detailed instructions on how to use the various commands available in the bot.
 
-- `/prodia`: Similar to `/image`, this command also generates images from text descriptions. However, it uses a different provider (Prodia) to create the images. This could offer a different style or interpretation of the text descriptions compared to the default method.
+- **/start**: Displays the help information, offering a comprehensive list of available commands and their functionalities. This command is essential for users to quickly understand how to interact with the bot.
 
-- `/audio`: Converts text to speech. Users can input text, and the bot will generate an audio file that reads out the text. This can be useful for listening to descriptions, instructions, or any text content.
+- **/chat**: Initiate a natural language conversation with the AI. This command allows users to engage in interactive dialogues, ask questions, or make requests.
 
-- `/sintro`: Allows users to set a new text for the chat intro. This can be used to customize the greeting message that users see when they start a new chat session with the bot.
+- **/image**: Generates images from textual descriptions using the default provider. This feature enables users to visualize ideas or concepts through images.
 
-- `/svoice`: Lets users set a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
+- **/prodia**: Generates images from textual descriptions using the Prodia provider. This command offers a unique style or interpretation of the text descriptions compared to the default method.
 
-- `/awesome`: Sets an awesome prompt as the introductory message for the chat. This could be a motivational quote, a fun fact, or any other type of prompt that might inspire or engage users in their interactions with the bot.
+- **/audio**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
 
-- `/history`: Checks the chat history. This command allows users to view the history of their chats with the bot. It can be useful for users who want to review past interactions or find specific information from previous conversations.
+- **/intro**: Sets a new text for the chat intro. This command allows users to customize the chat introductory prompt which serves as a guide in the human-AI engagement.
 
-- `/settings`: Checks the current settings of the bot. This command provides users with an overview of the bot's current configuration, including any custom settings they have applied.
+- **/voice**: Sets a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
 
-- `/reset`: Starts a new chat thread. This command resets the chat history and starts a new conversation thread. It's useful for users who want to start fresh or who want to clear their chat history for privacy reasons.
+- **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
 
-- `/myid`: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for any reason, such as setting up bot admin.
+- **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of them.
+
+- **/history**: Provides users with the ability to view the history of their chats with the bot. This command is useful for reviewing past interactions or finding specific information from previous conversations.
+
+- **/settings**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
+
+- **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
+
+- **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
+
+- `any other text or command>`: An alias for `/chat`, allowing users to continue with text chat.
+
+
+### Administrative Commands
 
-- `/default`: Chat with AI. This command is essentially an alias for `/chat`, allowing users to initiate a chat session with the AI using a different command.
 
 ### Administrative Commands
 
 - `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
 
 - `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
 
-- `/drop`: Clears the entire chat table. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data.
+- `/drop`: Clears the entire chat table and bot logs. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data and current contents of log file.
 
 - `/sql`: Allows running SQL statements against the database. This command provides a way for administrators to directly interact with the bot's database using SQL queries. It's a powerful tool for managing and analyzing the bot's data but should be used with caution to avoid unintended data loss or corruption.
 
+- `/logs`: Checks the logs. This command is used to access the bot's logs, which can provide insights into the bot's activity, errors, and user interactions. It's a valuable tool for monitoring and troubleshooting the bot's performance.
+
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
 
 ## License
 
 `pytgpt-bot` is open-source and available under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code as you see fit.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.6 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.7 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -36,61 +36,61 @@
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the server
 `python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
-Features ### Commands - `/help`: This command displays the help information,
-providing users with a list of available commands and a brief description of
-what each command does. It's a useful way for users to quickly understand how
-to interact with the bot. - `/chat`: Allows users to engage in natural language
-conversations with the AI. This command initiates a chat session where users
-can ask questions, make requests, or simply chat with the AI. - `/image`: This
-command is used to generate images from text descriptions. Users can input a
-text description, and the bot will attempt to create an image based on that
-description. This feature can be particularly useful for visualizing ideas or
-concepts. - `/prodia`: Similar to `/image`, this command also generates images
-from text descriptions. However, it uses a different provider (Prodia) to
-create the images. This could offer a different style or interpretation of the
-text descriptions compared to the default method. - `/audio`: Converts text to
-speech. Users can input text, and the bot will generate an audio file that
-reads out the text. This can be useful for listening to descriptions,
-instructions, or any text content. - `/sintro`: Allows users to set a new text
-for the chat intro. This can be used to customize the greeting message that
-users see when they start a new chat session with the bot. - `/svoice`: Lets
-users set a new voice for speech synthesis. This command enables users to
-choose from different voices for the AI to use when generating audio from text.
-- `/awesome`: Sets an awesome prompt as the introductory message for the chat.
-This could be a motivational quote, a fun fact, or any other type of prompt
-that might inspire or engage users in their interactions with the bot. - `/
-history`: Checks the chat history. This command allows users to view the
-history of their chats with the bot. It can be useful for users who want to
-review past interactions or find specific information from previous
-conversations. - `/settings`: Checks the current settings of the bot. This
-command provides users with an overview of the bot's current configuration,
-including any custom settings they have applied. - `/reset`: Starts a new chat
-thread. This command resets the chat history and starts a new conversation
-thread. It's useful for users who want to start fresh or who want to clear
-their chat history for privacy reasons. - `/myid`: Echoes the user's Telegram
-ID. This command is useful for users who need to know their Telegram ID for any
-reason, such as setting up bot admin. - `/default`: Chat with AI. This command
-is essentially an alias for `/chat`, allowing users to initiate a chat session
-with the AI using a different command. ### Administrative Commands - `/clear`:
-Clears all chats. This command is used to remove all chat data from the bot's
-database. It's a powerful command that should be used with caution, as it will
-delete all chat history. - `/total`: Shows the total number of chats available.
-This command provides an overview of the current chat data stored in the bot's
-database, helping administrators understand the volume of interactions the bot
-has had. - `/drop`: Clears the entire chat table. Similar to `/clear`, this
-command removes all data from the chat table in the database. It's a more
-drastic measure than `/clear`, as it completely wipes out all chat data. - `/
-sql`: Allows running SQL statements against the database. This command provides
-a way for administrators to directly interact with the bot's database using SQL
-queries. It's a powerful tool for managing and analyzing the bot's data but
-should be used with caution to avoid unintended data loss or corruption. ##
+Features ### Commands ### Usage Information This section provides detailed
+instructions on how to use the various commands available in the bot. - **/
+start**: Displays the help information, offering a comprehensive list of
+available commands and their functionalities. This command is essential for
+users to quickly understand how to interact with the bot. - **/chat**: Initiate
+a natural language conversation with the AI. This command allows users to
+engage in interactive dialogues, ask questions, or make requests. - **/image**:
+Generates images from textual descriptions using the default provider. This
+feature enables users to visualize ideas or concepts through images. - **/
+prodia**: Generates images from textual descriptions using the Prodia provider.
+This command offers a unique style or interpretation of the text descriptions
+compared to the default method. - **/audio**: Converts text to speech,
+providing users with the ability to listen to descriptions, instructions, or
+any text content read out by the AI. - **/intro**: Sets a new text for the chat
+intro. This command allows users to customize the chat introductory prompt
+which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
+voice for speech synthesis. This command enables users to choose from different
+voices for the AI to use when generating audio from text. - **/provider**: Sets
+a new chat provider. This command allows users to switch between different
+providers for various functionalities, such as `phind`, `llama2`, `koboldai`
+etc. - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of
+them. - **/history**: Provides users with the ability to view the history of
+their chats with the bot. This command is useful for reviewing past
+interactions or finding specific information from previous conversations. - **/
+settings**: Offers an overview of the bot's current configuration, including
+any custom settings applied by the user. - **/reset**: Resets the chat history
+and starts a new conversation thread. This command is useful for users who wish
+to start fresh or clear their chat history for privacy reasons. - **/myid**:
+Echoes the user's Telegram ID. This command is useful for users who need to
+know their Telegram ID for various purposes, such as setting up bot admin. -
+`any other text or command>`: An alias for `/chat`, allowing users to continue
+with text chat. ### Administrative Commands ### Administrative Commands - `/
+clear`: Clears all chats. This command is used to remove all chat data from the
+bot's database. It's a powerful command that should be used with caution, as it
+will delete all chat history. - `/total`: Shows the total number of chats
+available. This command provides an overview of the current chat data stored in
+the bot's database, helping administrators understand the volume of
+interactions the bot has had. - `/drop`: Clears the entire chat table and bot
+logs. Similar to `/clear`, this command removes all data from the chat table in
+the database. It's a more drastic measure than `/clear`, as it completely wipes
+out all chat data and current contents of log file. - `/sql`: Allows running
+SQL statements against the database. This command provides a way for
+administrators to directly interact with the bot's database using SQL queries.
+It's a powerful tool for managing and analyzing the bot's data but should be
+used with caution to avoid unintended data loss or corruption. - `/logs`:
+Checks the logs. This command is used to access the bot's logs, which can
+provide insights into the bot's activity, errors, and user interactions. It's a
+valuable tool for monitoring and troubleshooting the bot's performance. ##
 Support and Feedback If you have any questions, feedback, or suggestions for
 `pytgpt`, please feel free to reach out. Your input is valuable in helping us
 improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
 source and available under the [MIT License](LICENSE). Feel free to use,
 modify, and distribute the code as you see fit. --- Thank you for using
 `pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.0.6/setup.py` & `pytgpt_bot-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.0.6",
+    version="0.0.7",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Telegram bot for text generation, text-to-image and text-to-audio conversions.",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
```

