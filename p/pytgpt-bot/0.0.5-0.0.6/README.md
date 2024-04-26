# Comparing `tmp/pytgpt_bot-0.0.5.tar.gz` & `tmp/pytgpt_bot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.0.5.tar", last modified: Thu Apr 25 13:11:00 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.0.6.tar", last modified: Thu Apr 25 18:07:06 2024, max compression
```

## Comparing `pytgpt_bot-0.0.5.tar` & `pytgpt_bot-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:11:00.713943 pytgpt_bot-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8387 2024-04-25 13:11:00.709943 pytgpt_bot-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:11:00.709943 pytgpt_bot-0.0.5/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:11:00.709943 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8387 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:11:00.713943 pytgpt_bot-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:07:06.625783 pytgpt_bot-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-25 18:07:06.625783 pytgpt_bot-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:07:06.625783 pytgpt_bot-0.0.6/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/pytgpt_bot/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:07:06.625783 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 18:07:06.000000 pytgpt_bot-0.0.6/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:07:06.625783 pytgpt_bot-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-25 18:06:49.000000 pytgpt_bot-0.0.6/setup.py
```

### Comparing `pytgpt_bot-0.0.5/LICENSE` & `pytgpt_bot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.5/PKG-INFO` & `pytgpt_bot-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -30,15 +30,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytelegrambotapi==4.17.0
 Requires-Dist: python-tgpt==0.6.6
 Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: appdirs==1.4.4
 Requires-Dist: click==8.1.3
 
 <p align="center">
 <a href="https://github.com/Simatwa/pytgpt-bot/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=MIT&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt"/></a>
 <a href="https://pypi.org/project/pytgpt-bot"><img alt="PyPi" src="https://img.shields.io/pypi/v/pytgpt-bot?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
@@ -47,15 +46,15 @@
 <a href="https://github.com/Simatwa/pytgpt-bot/releases"><img src="https://img.shields.io/github/v/release/Simatwa/pytgpt-bot?color=success&label=Release&logo=github" alt="Latest release"></img></a> 
 -->
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/pytgpt-bot"/></a>
 <a href="https://wakatime.com/badge/github/Simatwa/pytgpt-bot"><img src="https://wakatime.com/badge/github/Simatwa/pytgpt-bot.svg" alt="wakatime"></a>
 </p>
 
 <h1 align="center">
-Welcome to <a href="https://github.com/Simatwa/pytgpt-bot">pytgpt-bot</a>
+Welcome to <a href="https://t.me/pytgpt_bot">pytgpt-bot</a>
 </h1>
 
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/python-tgpt), a powerful tool designed to enhance your interactions with AI. This bot is built on the robust foundation of the `pyTelegramBotAPI` and offers a wide range of features to make your experience with AI more engaging and interactive. Whether you're looking to chat with AI, generate images and audio from text, `pytgpt-bot` has got you covered.
 
 ## Prerequisites
 
 - [x] [Python>=3.10](https://python.org)
@@ -86,81 +85,51 @@
 
 Alternatively, using CLI interface::
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
-### 1. Chat with AI
+### Commands
 
-- **Command**: `/chat`
-- **Description**: Engage in a conversation with AI. This feature allows you to interact with the bot in a natural, conversational manner.
+- `/help`: This command displays the help information, providing users with a list of available commands and a brief description of what each command does. It's a useful way for users to quickly understand how to interact with the bot.
 
-### 2. Generate Images from Text
+- `/chat`: Allows users to engage in natural language conversations with the AI. This command initiates a chat session where users can ask questions, make requests, or simply chat with the AI.
 
-- **Command**: `/image`
-- **Description**: Generate images from text descriptions. This feature uses AI to create visual representations of your text inputs, making it a fun and creative way to explore the capabilities of AI.
+- `/image`: This command is used to generate images from text descriptions. Users can input a text description, and the bot will attempt to create an image based on that description. This feature can be particularly useful for visualizing ideas or concepts.
 
-- **Variant**: `/prodia`
-- **Description**: Generate images from text descriptions using the Prodia AI model. This variant offers a different style of image generation, providing a unique twist to your creative endeavors.
+- `/prodia`: Similar to `/image`, this command also generates images from text descriptions. However, it uses a different provider (Prodia) to create the images. This could offer a different style or interpretation of the text descriptions compared to the default method.
 
-### 3. Generate Audio from Text
+- `/audio`: Converts text to speech. Users can input text, and the bot will generate an audio file that reads out the text. This can be useful for listening to descriptions, instructions, or any text content.
 
-- **Command**: `/audio`
-- **Description**: Generate audio from text. This feature allows you to convert your text inputs into spoken words, enabling you to listen to the AI's voice or use the audio for other purposes.
+- `/sintro`: Allows users to set a new text for the chat intro. This can be used to customize the greeting message that users see when they start a new chat session with the bot.
 
-### 4. Check Current Chat Introduction
+- `/svoice`: Lets users set a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
 
-- **Command**: `/intro`
-- **Description**: Check the current chat introduction. This feature allows you to view the introduction text set for the current chat, providing context and setting the tone for your interactions.
+- `/awesome`: Sets an awesome prompt as the introductory message for the chat. This could be a motivational quote, a fun fact, or any other type of prompt that might inspire or engage users in their interactions with the bot.
 
-### 5. Check Chat History
+- `/history`: Checks the chat history. This command allows users to view the history of their chats with the bot. It can be useful for users who want to review past interactions or find specific information from previous conversations.
 
-- **Command**: `/history`
-- **Description**: Check the chat history. This feature allows you to review past interactions within the chat, helping you to recall previous discussions and decisions.
+- `/settings`: Checks the current settings of the bot. This command provides users with an overview of the bot's current configuration, including any custom settings they have applied.
 
-### 6. Set New Value for Chat Introduction
+- `/reset`: Starts a new chat thread. This command resets the chat history and starts a new conversation thread. It's useful for users who want to start fresh or who want to clear their chat history for privacy reasons.
 
-- **Command**: `/sintro`
-- **Description**: Set a new value for the chat introduction. This feature enables you to customize the introduction text for the current chat, allowing you to tailor the conversation to your preferences.
+- `/myid`: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for any reason, such as setting up bot admin.
 
-### 7. Start New Chat Thread
+- `/default`: Chat with AI. This command is essentially an alias for `/chat`, allowing users to initiate a chat session with the AI using a different command.
 
-- **Command**: `/reset`
-- **Description**: Start a new chat thread. This feature allows you to begin a fresh conversation with the bot, resetting the chat history and allowing for a new start.
+### Administrative Commands
 
-### 8. Echo Your Telegram ID
+- `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
 
-- **Command**: `/myid`
-- **Description**: Echo your Telegram ID. This feature provides you with your unique Telegram ID, useful for personalized interactions or for troubleshooting purposes and configuring admin.
+- `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
 
-### 9. Clear chat data
+- `/drop`: Clears the entire chat table. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data.
 
-- **Command**: `/clear_chats`
-- **Description**: This is an administrative command for deleting all entries of chat database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 10. Check total Chat
-
-- **Command**: `/total_chats`
-- **Description**: This is an administrative command for checking total chat records. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 11. Drop entire chat
-
-- **Command**: `/drop_chats`
-- **Description**: This is an administrative command that **drops** entire chat table and create new one. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 12. Run sql statements
-
-- **Command**: `/sql`
-- **Description**: This is an administrative command for running **SQL STATEMENTS** against the database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 12. Default Chat with AI
-
-- **Command**: `<Any other text>`
-- **Description**: Engage in a default chat with AI. This command is a shortcut to the `/chat` command, offering a quick and straightforward way to start a conversation with the bot.
+- `/sql`: Allows running SQL statements against the database. This command provides a way for administrators to directly interact with the bot's database using SQL queries. It's a powerful tool for managing and analyzing the bot's data but should be used with caution to avoid unintended data loss or corruption.
 
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.5 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.6 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -17,15 +17,15 @@
 Python Modules Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pytelegrambotapi==4.17.0 Requires-Dist: python-tgpt==0.6.6 Requires-Dist:
-python-dotenv==1.0.0 Requires-Dist: appdirs==1.4.4 Requires-Dist: click==8.1.3
+python-dotenv==1.0.0 Requires-Dist: click==8.1.3
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/
    _a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_g_p_t_-_b_o_t_]
                                   _[_w_a_k_a_t_i_m_e_]
                       ************ WWeellccoommee ttoo _pp_yy_tt_gg_pp_tt_--_bb_oo_tt ************
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/
 python-tgpt), a powerful tool designed to enhance your interactions with AI.
 This bot is built on the robust foundation of the `pyTelegramBotAPI` and offers
@@ -36,61 +36,61 @@
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the server
 `python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
-Features ### 1. Chat with AI - **Command**: `/chat` - **Description**: Engage
-in a conversation with AI. This feature allows you to interact with the bot in
-a natural, conversational manner. ### 2. Generate Images from Text -
-**Command**: `/image` - **Description**: Generate images from text
-descriptions. This feature uses AI to create visual representations of your
-text inputs, making it a fun and creative way to explore the capabilities of
-AI. - **Variant**: `/prodia` - **Description**: Generate images from text
-descriptions using the Prodia AI model. This variant offers a different style
-of image generation, providing a unique twist to your creative endeavors. ###
-3. Generate Audio from Text - **Command**: `/audio` - **Description**: Generate
-audio from text. This feature allows you to convert your text inputs into
-spoken words, enabling you to listen to the AI's voice or use the audio for
-other purposes. ### 4. Check Current Chat Introduction - **Command**: `/intro`
-- **Description**: Check the current chat introduction. This feature allows you
-to view the introduction text set for the current chat, providing context and
-setting the tone for your interactions. ### 5. Check Chat History -
-**Command**: `/history` - **Description**: Check the chat history. This feature
-allows you to review past interactions within the chat, helping you to recall
-previous discussions and decisions. ### 6. Set New Value for Chat Introduction
-- **Command**: `/sintro` - **Description**: Set a new value for the chat
-introduction. This feature enables you to customize the introduction text for
-the current chat, allowing you to tailor the conversation to your preferences.
-### 7. Start New Chat Thread - **Command**: `/reset` - **Description**: Start a
-new chat thread. This feature allows you to begin a fresh conversation with the
-bot, resetting the chat history and allowing for a new start. ### 8. Echo Your
-Telegram ID - **Command**: `/myid` - **Description**: Echo your Telegram ID.
-This feature provides you with your unique Telegram ID, useful for personalized
-interactions or for troubleshooting purposes and configuring admin. ### 9.
-Clear chat data - **Command**: `/clear_chats` - **Description**: This is an
-administrative command for deleting all entries of chat database. The user's
-Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
-pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-### 10. Check total Chat - **Command**: `/total_chats` - **Description**: This
-is an administrative command for checking total chat records. The user's
-Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
-pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-### 11. Drop entire chat - **Command**: `/drop_chats` - **Description**: This
-is an administrative command that **drops** entire chat table and create new
-one. The user's Telegram ID must match the one set at the [.env](https://
-github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/
-env#L2) config file. ### 12. Run sql statements - **Command**: `/sql` -
-**Description**: This is an administrative command for running **SQL
-STATEMENTS** against the database. The user's Telegram ID must match the one
-set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/
-7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file. ### 12. Default
-Chat with AI - **Command**: `` - **Description**: Engage in a default chat with
-AI. This command is a shortcut to the `/chat` command, offering a quick and
-straightforward way to start a conversation with the bot. ## Support and
-Feedback If you have any questions, feedback, or suggestions for `pytgpt`,
-please feel free to reach out. Your input is valuable in helping us improve and
-expand the bot's capabilities. ## License `pytgpt-bot` is open-source and
-available under the [MIT License](LICENSE). Feel free to use, modify, and
-distribute the code as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy
-your AI-powered interactions!
+Features ### Commands - `/help`: This command displays the help information,
+providing users with a list of available commands and a brief description of
+what each command does. It's a useful way for users to quickly understand how
+to interact with the bot. - `/chat`: Allows users to engage in natural language
+conversations with the AI. This command initiates a chat session where users
+can ask questions, make requests, or simply chat with the AI. - `/image`: This
+command is used to generate images from text descriptions. Users can input a
+text description, and the bot will attempt to create an image based on that
+description. This feature can be particularly useful for visualizing ideas or
+concepts. - `/prodia`: Similar to `/image`, this command also generates images
+from text descriptions. However, it uses a different provider (Prodia) to
+create the images. This could offer a different style or interpretation of the
+text descriptions compared to the default method. - `/audio`: Converts text to
+speech. Users can input text, and the bot will generate an audio file that
+reads out the text. This can be useful for listening to descriptions,
+instructions, or any text content. - `/sintro`: Allows users to set a new text
+for the chat intro. This can be used to customize the greeting message that
+users see when they start a new chat session with the bot. - `/svoice`: Lets
+users set a new voice for speech synthesis. This command enables users to
+choose from different voices for the AI to use when generating audio from text.
+- `/awesome`: Sets an awesome prompt as the introductory message for the chat.
+This could be a motivational quote, a fun fact, or any other type of prompt
+that might inspire or engage users in their interactions with the bot. - `/
+history`: Checks the chat history. This command allows users to view the
+history of their chats with the bot. It can be useful for users who want to
+review past interactions or find specific information from previous
+conversations. - `/settings`: Checks the current settings of the bot. This
+command provides users with an overview of the bot's current configuration,
+including any custom settings they have applied. - `/reset`: Starts a new chat
+thread. This command resets the chat history and starts a new conversation
+thread. It's useful for users who want to start fresh or who want to clear
+their chat history for privacy reasons. - `/myid`: Echoes the user's Telegram
+ID. This command is useful for users who need to know their Telegram ID for any
+reason, such as setting up bot admin. - `/default`: Chat with AI. This command
+is essentially an alias for `/chat`, allowing users to initiate a chat session
+with the AI using a different command. ### Administrative Commands - `/clear`:
+Clears all chats. This command is used to remove all chat data from the bot's
+database. It's a powerful command that should be used with caution, as it will
+delete all chat history. - `/total`: Shows the total number of chats available.
+This command provides an overview of the current chat data stored in the bot's
+database, helping administrators understand the volume of interactions the bot
+has had. - `/drop`: Clears the entire chat table. Similar to `/clear`, this
+command removes all data from the chat table in the database. It's a more
+drastic measure than `/clear`, as it completely wipes out all chat data. - `/
+sql`: Allows running SQL statements against the database. This command provides
+a way for administrators to directly interact with the bot's database using SQL
+queries. It's a powerful tool for managing and analyzing the bot's data but
+should be used with caution to avoid unintended data loss or corruption. ##
+Support and Feedback If you have any questions, feedback, or suggestions for
+`pytgpt`, please feel free to reach out. Your input is valuable in helping us
+improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
+source and available under the [MIT License](LICENSE). Feel free to use,
+modify, and distribute the code as you see fit. --- Thank you for using
+`pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.0.5/README.md` & `pytgpt_bot-0.0.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <a href="https://github.com/Simatwa/pytgpt-bot/releases"><img src="https://img.shields.io/github/v/release/Simatwa/pytgpt-bot?color=success&label=Release&logo=github" alt="Latest release"></img></a> 
 -->
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/pytgpt-bot"/></a>
 <a href="https://wakatime.com/badge/github/Simatwa/pytgpt-bot"><img src="https://wakatime.com/badge/github/Simatwa/pytgpt-bot.svg" alt="wakatime"></a>
 </p>
 
 <h1 align="center">
-Welcome to <a href="https://github.com/Simatwa/pytgpt-bot">pytgpt-bot</a>
+Welcome to <a href="https://t.me/pytgpt_bot">pytgpt-bot</a>
 </h1>
 
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/python-tgpt), a powerful tool designed to enhance your interactions with AI. This bot is built on the robust foundation of the `pyTelegramBotAPI` and offers a wide range of features to make your experience with AI more engaging and interactive. Whether you're looking to chat with AI, generate images and audio from text, `pytgpt-bot` has got you covered.
 
 ## Prerequisites
 
 - [x] [Python>=3.10](https://python.org)
@@ -47,81 +47,51 @@
 
 Alternatively, using CLI interface::
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
-### 1. Chat with AI
+### Commands
 
-- **Command**: `/chat`
-- **Description**: Engage in a conversation with AI. This feature allows you to interact with the bot in a natural, conversational manner.
+- `/help`: This command displays the help information, providing users with a list of available commands and a brief description of what each command does. It's a useful way for users to quickly understand how to interact with the bot.
 
-### 2. Generate Images from Text
+- `/chat`: Allows users to engage in natural language conversations with the AI. This command initiates a chat session where users can ask questions, make requests, or simply chat with the AI.
 
-- **Command**: `/image`
-- **Description**: Generate images from text descriptions. This feature uses AI to create visual representations of your text inputs, making it a fun and creative way to explore the capabilities of AI.
+- `/image`: This command is used to generate images from text descriptions. Users can input a text description, and the bot will attempt to create an image based on that description. This feature can be particularly useful for visualizing ideas or concepts.
 
-- **Variant**: `/prodia`
-- **Description**: Generate images from text descriptions using the Prodia AI model. This variant offers a different style of image generation, providing a unique twist to your creative endeavors.
+- `/prodia`: Similar to `/image`, this command also generates images from text descriptions. However, it uses a different provider (Prodia) to create the images. This could offer a different style or interpretation of the text descriptions compared to the default method.
 
-### 3. Generate Audio from Text
+- `/audio`: Converts text to speech. Users can input text, and the bot will generate an audio file that reads out the text. This can be useful for listening to descriptions, instructions, or any text content.
 
-- **Command**: `/audio`
-- **Description**: Generate audio from text. This feature allows you to convert your text inputs into spoken words, enabling you to listen to the AI's voice or use the audio for other purposes.
+- `/sintro`: Allows users to set a new text for the chat intro. This can be used to customize the greeting message that users see when they start a new chat session with the bot.
 
-### 4. Check Current Chat Introduction
+- `/svoice`: Lets users set a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
 
-- **Command**: `/intro`
-- **Description**: Check the current chat introduction. This feature allows you to view the introduction text set for the current chat, providing context and setting the tone for your interactions.
+- `/awesome`: Sets an awesome prompt as the introductory message for the chat. This could be a motivational quote, a fun fact, or any other type of prompt that might inspire or engage users in their interactions with the bot.
 
-### 5. Check Chat History
+- `/history`: Checks the chat history. This command allows users to view the history of their chats with the bot. It can be useful for users who want to review past interactions or find specific information from previous conversations.
 
-- **Command**: `/history`
-- **Description**: Check the chat history. This feature allows you to review past interactions within the chat, helping you to recall previous discussions and decisions.
+- `/settings`: Checks the current settings of the bot. This command provides users with an overview of the bot's current configuration, including any custom settings they have applied.
 
-### 6. Set New Value for Chat Introduction
+- `/reset`: Starts a new chat thread. This command resets the chat history and starts a new conversation thread. It's useful for users who want to start fresh or who want to clear their chat history for privacy reasons.
 
-- **Command**: `/sintro`
-- **Description**: Set a new value for the chat introduction. This feature enables you to customize the introduction text for the current chat, allowing you to tailor the conversation to your preferences.
+- `/myid`: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for any reason, such as setting up bot admin.
 
-### 7. Start New Chat Thread
+- `/default`: Chat with AI. This command is essentially an alias for `/chat`, allowing users to initiate a chat session with the AI using a different command.
 
-- **Command**: `/reset`
-- **Description**: Start a new chat thread. This feature allows you to begin a fresh conversation with the bot, resetting the chat history and allowing for a new start.
+### Administrative Commands
 
-### 8. Echo Your Telegram ID
+- `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
 
-- **Command**: `/myid`
-- **Description**: Echo your Telegram ID. This feature provides you with your unique Telegram ID, useful for personalized interactions or for troubleshooting purposes and configuring admin.
+- `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
 
-### 9. Clear chat data
+- `/drop`: Clears the entire chat table. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data.
 
-- **Command**: `/clear_chats`
-- **Description**: This is an administrative command for deleting all entries of chat database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 10. Check total Chat
-
-- **Command**: `/total_chats`
-- **Description**: This is an administrative command for checking total chat records. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 11. Drop entire chat
-
-- **Command**: `/drop_chats`
-- **Description**: This is an administrative command that **drops** entire chat table and create new one. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 12. Run sql statements
-
-- **Command**: `/sql`
-- **Description**: This is an administrative command for running **SQL STATEMENTS** against the database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 12. Default Chat with AI
-
-- **Command**: `<Any other text>`
-- **Description**: Engage in a default chat with AI. This command is a shortcut to the `/chat` command, offering a quick and straightforward way to start a conversation with the bot.
+- `/sql`: Allows running SQL statements against the database. This command provides a way for administrators to directly interact with the bot's database using SQL queries. It's a powerful tool for managing and analyzing the bot's data but should be used with caution to avoid unintended data loss or corruption.
 
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
 
 ## License
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
-Features ### 1. Chat with AI - **Command**: `/chat` - **Description**: Engage
-in a conversation with AI. This feature allows you to interact with the bot in
-a natural, conversational manner. ### 2. Generate Images from Text -
-**Command**: `/image` - **Description**: Generate images from text
-descriptions. This feature uses AI to create visual representations of your
-text inputs, making it a fun and creative way to explore the capabilities of
-AI. - **Variant**: `/prodia` - **Description**: Generate images from text
-descriptions using the Prodia AI model. This variant offers a different style
-of image generation, providing a unique twist to your creative endeavors. ###
-3. Generate Audio from Text - **Command**: `/audio` - **Description**: Generate
-audio from text. This feature allows you to convert your text inputs into
-spoken words, enabling you to listen to the AI's voice or use the audio for
-other purposes. ### 4. Check Current Chat Introduction - **Command**: `/intro`
-- **Description**: Check the current chat introduction. This feature allows you
-to view the introduction text set for the current chat, providing context and
-setting the tone for your interactions. ### 5. Check Chat History -
-**Command**: `/history` - **Description**: Check the chat history. This feature
-allows you to review past interactions within the chat, helping you to recall
-previous discussions and decisions. ### 6. Set New Value for Chat Introduction
-- **Command**: `/sintro` - **Description**: Set a new value for the chat
-introduction. This feature enables you to customize the introduction text for
-the current chat, allowing you to tailor the conversation to your preferences.
-### 7. Start New Chat Thread - **Command**: `/reset` - **Description**: Start a
-new chat thread. This feature allows you to begin a fresh conversation with the
-bot, resetting the chat history and allowing for a new start. ### 8. Echo Your
-Telegram ID - **Command**: `/myid` - **Description**: Echo your Telegram ID.
-This feature provides you with your unique Telegram ID, useful for personalized
-interactions or for troubleshooting purposes and configuring admin. ### 9.
-Clear chat data - **Command**: `/clear_chats` - **Description**: This is an
-administrative command for deleting all entries of chat database. The user's
-Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
-pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-### 10. Check total Chat - **Command**: `/total_chats` - **Description**: This
-is an administrative command for checking total chat records. The user's
-Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
-pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-### 11. Drop entire chat - **Command**: `/drop_chats` - **Description**: This
-is an administrative command that **drops** entire chat table and create new
-one. The user's Telegram ID must match the one set at the [.env](https://
-github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/
-env#L2) config file. ### 12. Run sql statements - **Command**: `/sql` -
-**Description**: This is an administrative command for running **SQL
-STATEMENTS** against the database. The user's Telegram ID must match the one
-set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/
-7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file. ### 12. Default
-Chat with AI - **Command**: `` - **Description**: Engage in a default chat with
-AI. This command is a shortcut to the `/chat` command, offering a quick and
-straightforward way to start a conversation with the bot. ## Support and
-Feedback If you have any questions, feedback, or suggestions for `pytgpt`,
-please feel free to reach out. Your input is valuable in helping us improve and
-expand the bot's capabilities. ## License `pytgpt-bot` is open-source and
-available under the [MIT License](LICENSE). Feel free to use, modify, and
-distribute the code as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy
-your AI-powered interactions!
+Features ### Commands - `/help`: This command displays the help information,
+providing users with a list of available commands and a brief description of
+what each command does. It's a useful way for users to quickly understand how
+to interact with the bot. - `/chat`: Allows users to engage in natural language
+conversations with the AI. This command initiates a chat session where users
+can ask questions, make requests, or simply chat with the AI. - `/image`: This
+command is used to generate images from text descriptions. Users can input a
+text description, and the bot will attempt to create an image based on that
+description. This feature can be particularly useful for visualizing ideas or
+concepts. - `/prodia`: Similar to `/image`, this command also generates images
+from text descriptions. However, it uses a different provider (Prodia) to
+create the images. This could offer a different style or interpretation of the
+text descriptions compared to the default method. - `/audio`: Converts text to
+speech. Users can input text, and the bot will generate an audio file that
+reads out the text. This can be useful for listening to descriptions,
+instructions, or any text content. - `/sintro`: Allows users to set a new text
+for the chat intro. This can be used to customize the greeting message that
+users see when they start a new chat session with the bot. - `/svoice`: Lets
+users set a new voice for speech synthesis. This command enables users to
+choose from different voices for the AI to use when generating audio from text.
+- `/awesome`: Sets an awesome prompt as the introductory message for the chat.
+This could be a motivational quote, a fun fact, or any other type of prompt
+that might inspire or engage users in their interactions with the bot. - `/
+history`: Checks the chat history. This command allows users to view the
+history of their chats with the bot. It can be useful for users who want to
+review past interactions or find specific information from previous
+conversations. - `/settings`: Checks the current settings of the bot. This
+command provides users with an overview of the bot's current configuration,
+including any custom settings they have applied. - `/reset`: Starts a new chat
+thread. This command resets the chat history and starts a new conversation
+thread. It's useful for users who want to start fresh or who want to clear
+their chat history for privacy reasons. - `/myid`: Echoes the user's Telegram
+ID. This command is useful for users who need to know their Telegram ID for any
+reason, such as setting up bot admin. - `/default`: Chat with AI. This command
+is essentially an alias for `/chat`, allowing users to initiate a chat session
+with the AI using a different command. ### Administrative Commands - `/clear`:
+Clears all chats. This command is used to remove all chat data from the bot's
+database. It's a powerful command that should be used with caution, as it will
+delete all chat history. - `/total`: Shows the total number of chats available.
+This command provides an overview of the current chat data stored in the bot's
+database, helping administrators understand the volume of interactions the bot
+has had. - `/drop`: Clears the entire chat table. Similar to `/clear`, this
+command removes all data from the chat table in the database. It's a more
+drastic measure than `/clear`, as it completely wipes out all chat data. - `/
+sql`: Allows running SQL statements against the database. This command provides
+a way for administrators to directly interact with the bot's database using SQL
+queries. It's a powerful tool for managing and analyzing the bot's data but
+should be used with caution to avoid unintended data loss or corruption. ##
+Support and Feedback If you have any questions, feedback, or suggestions for
+`pytgpt`, please feel free to reach out. Your input is valuable in helping us
+improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
+source and available under the [MIT License](LICENSE). Feel free to use,
+modify, and distribute the code as you see fit. --- Thank you for using
+`pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.0.5/pytgpt_bot/cli.py` & `pytgpt_bot-0.0.6/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.5/pytgpt_bot/config.py` & `pytgpt_bot-0.0.6/pytgpt_bot/config.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.5/pytgpt_bot/db.py` & `pytgpt_bot-0.0.6/pytgpt_bot/db.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sqlite3
 from .config import admin_id
 from .config import path_to_db
 from functools import wraps
 import logging
 import typing
 from pytgpt.utils import Conversation
+from pytgpt.utils import Audio
 
 
 def exception_handler(func):
 
     @wraps(func)
     def decorator(*args, **kwargs):
         try:
@@ -28,15 +29,17 @@
         """Creates database"""
         conn = sqlite3.connect(path_to_db)
         conn.execute(
             f"""
         CREATE TABLE IF NOT EXISTS Chat(
             Id INTEGER PRIMARY KEY,
             Intro TEXT DEFAULT "{Conversation.intro}",
-            History TEXT);
+            History TEXT DEFAULT "",
+            Voice TEXT DEFAULT "Brian"
+            );
         """
         )
         conn.commit()
 
     @staticmethod
     @exception_handler
     def insert(**kwargs):
@@ -146,27 +149,32 @@
     @property
     def record(self) -> typing.Dict[str, typing.Union[int, str]]:
         """User data
 
         Returns:
             typing.Dict[str, typing.Union[int, str]]: Records
         """
-        id, intro, history = Chat.read(id=self.id, fetchone=True)
-        return dict(id=id, intro=intro, history=history)
+        id, intro, history, voice = Chat.read(id=self.id, fetchone=True)
+        return dict(id=id, intro=intro, history=history, voice=voice)
 
     @property
     def chat_history(self) -> typing.Union[str, None]:
         """User's chat history"""
         return self.record.get("history")
 
     @property
     def chat_intro(self) -> str:
         """User's chat intro"""
         return self.record.get("intro")
 
+    @property
+    def chat_voice(self) -> typing.Union[str, None]:
+        """User's speech voice"""
+        return self.record.get("voice")
+
     def update_history(self, data: str):
         """Update chat history
 
         Args:
             data (str): New history
         """
         Chat.update(
@@ -183,14 +191,26 @@
         """
         Chat.update(
             self.id,
             field="intro",
             data=data,
         )
 
+    def update_voice(self, data: str):
+        """Update speech voice
+
+        Args:
+            data (str): New voice.
+        """
+        Chat.update(
+            self.id,
+            field="voice",
+            data=data,
+        )
+
     def delete(self):
         """Delete current user account"""
         Chat.delete(self.id)
 
 
 # import os
 # os.remove(path_to_db)
```

### Comparing `pytgpt_bot-0.0.5/pytgpt_bot/main.py` & `pytgpt_bot-0.0.6/pytgpt_bot/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 log_params = dict(
     format="%(asctime)s : %(levelname)s - %(message)s",
     datefmt="%d-%b-%Y %H:%M:%S",
     level=loglevel,
 )
 
+awesome_prompts: dict = AwesomePrompts().get_acts()
+awesome_prompts_keys: list = list(awesome_prompts.keys())
+
 if logfile:
     log_params["filename"] = logfile
 
 logging.basicConfig(**log_params)
 
 bot = telebot.TeleBot(bot_token, parse_mode="Markdown")
 
@@ -50,45 +53,64 @@
             try:
                 logging.info(
                     f"Serving user [{message.from_user.id}] ({message.from_user.full_name}) - Function [{func.__name__}]"
                 )
                 if admin and not User(message.from_user.id).is_admin:
                     return bot.reply_to(message, "Action restricted to admins only!")
 
-                if text and not message.text:
-                    return bot.reply_to(message, "Text is required.")
-
                 if message.text and message.text.startswith("/"):
                     message.text = " ".join(message.text.split(" ")[1:])
 
+                if text and not message.text:
+                    return bot.reply_to(message, "Text is required.")
+
                 return func(message)
             except Exception as e:
                 logging.error(f"Error on function - {func.__name__} - {e}")
+                logging.exception(e)
                 return bot.reply_to(
                     message, text="An error occured and could't complete that request."
                 )
 
         return decorator
 
     return main
 
 
+def send_long_text(message: telebot.types.Message, text: str):
+    """Send texts longer than 4096 long
+
+    Args:
+        message (telebot.types.Message): Message object.
+        text (str): Text to be sent.
+    """
+    max_length = 4096
+    if len(text) <= max_length:
+        bot.send_message(message.chat.id, text)
+    else:
+        parts = [text[i : i + max_length] for i in range(0, len(text), max_length)]
+        for part in parts:
+            bot.send_message(message.chat.id, part)
+
+
 @bot.message_handler(commands=["help", "start"])
 @handler_formatter()
 def home(message: telebot.types.Message):
     """
     Welcome to [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot).
     /help : Show this help info.
     /chat : Chat with AI.
     /imager : Generate image from text. (default)
     /prodia : Generate image from text. (Prodia)
     /audio : Generate audio from text.
-    /intro : Check current chat intro.
+    /sintro : Set new text for chat intro.
+    /svoice : Set new voice for speech synthesis.
+    /awesome : Set awesome prompt as intro.
     /history : Check chat history.
-    /sintro : Set new value for chat intro.
+    /settings : Check current settings.
     /reset : Start new chat thread.
     /myid : Echo your Telegram ID.
     /default : Chat with AI.
     """
 
     return bot.send_message(
         message.chat.id,
@@ -117,26 +139,97 @@
             message, "The chat introduction must be at least 10 characters long."
         )
     user = User(message.from_user.id)
     user.update_intro(intro)
     bot.reply_to(message, "New intro set successfully.")
 
 
-@bot.message_handler(commands=["intro"])
+@bot.message_handler(commands=["svoice"])
+@handler_formatter(text=False)
+def set_new_chat_intro(message: telebot.types.Message):
+    """Set new voice for speech synthesis"""
+    user_id: str = message.from_user.id
+    markup = telebot.types.InlineKeyboardMarkup(row_width=4)
+    make_item = lambda voice: telebot.types.InlineKeyboardButton(
+        voice, callback_data=f"{voice}:{user_id}"
+    )
+    markup.add(*map(make_item, audio_generator.all_voices))
+
+    return bot.send_message(message.chat.id, "Choose a voice:", reply_markup=markup)
+
+
+@bot.callback_query_handler(
+    func=lambda call: call.data.split(":")[0] in audio_generator.all_voices
+)
+def set_new_chat_intro_callback(call: telebot.types.CallbackQuery):
+    """Set new voice for speech synthesis callback handler"""
+    bot.delete_message(call.message.chat.id, call.message.id)
+    voice, user_id = call.data.split(":")
+    message = call.message
+    if not voice in audio_generator.all_voices:
+        return bot.reply_to(
+            message,
+            f"Voice '{voice}' is not one of : `({', '.join(audio_generator.all_voices)})`",
+        )
+    user = User(int(user_id))
+    user.update_voice(voice)
+    return bot.send_message(message.chat.id, f"New voice set : `{voice}`")
+
+
+@bot.message_handler(commands=["awesome"])
+@handler_formatter(text=False)
+def set_awesome_prompt_as_chat_intro(message: telebot.types.Message):
+    """Set awesome prompt as intro"""
+    user_id: str = message.from_user.id
+    markup = telebot.types.InlineKeyboardMarkup(row_width=4)
+    make_item = lambda awesome: telebot.types.InlineKeyboardButton(
+        awesome, callback_data=f"{awesome}:{user_id}"
+    )
+    markup.add(*map(make_item, awesome_prompts_keys))
+    return bot.send_message(message.chat.id, "Choose awesome:", reply_markup=markup)
+
+
+@bot.callback_query_handler(
+    func=lambda call: call.data.split(":")[0] in awesome_prompts_keys
+)
+def set_awesome_prompt_as_chat_intro_callback_handler(
+    call: telebot.types.CallbackQuery,
+):
+    """Set awesome prompt as intro callback handler"""
+    bot.delete_message(call.message.chat.id, call.message.id)
+    awesome_prompt, user_id = call.data.split(":")
+    user = User(int(user_id))
+    user.update_intro(awesome_prompts.get(awesome_prompt))
+    return bot.send_message(
+        call.message.chat.id,
+        f"""New awesome-intro set:
+```
+{awesome_prompts.get(awesome_prompt)}
+```.""",
+    )
+
+
+@bot.message_handler(commands=["settings"])
 @handler_formatter()
-def check_chat_intro(message: telebot.types.Message):
+def check_current_settings(message: telebot.types.Message):
+    """Check current user settings"""
     user = User(message.from_user.id)
-    return bot.reply_to(message, user.chat_intro)
+    current_user_settings = f"""
+    **Chat Length** : `{len(user.chat_history)}`
+    **Speech Voice** : `{user.chat_voice}`
+    **Chat Intro** : `{user.chat_intro}`
+    """
+    return bot.reply_to(message, current_user_settings)
 
 
 @bot.message_handler(commands=["history"])
 @handler_formatter()
 def check_chat_history(message: telebot.types.Message):
     user = User(message.from_user.id)
-    return bot.reply_to(message, user.chat_history or "Your chat history is empty.")
+    return send_long_text(message, user.chat_history or "Your chat history is empty.")
 
 
 @bot.message_handler(commands=["image", "img"])
 @handler_formatter(text=True)
 def text_to_image_default(message: telebot.types.Message):
     """Generate image using `image`"""
     generator_obj = image_generator.Imager(
@@ -165,15 +258,15 @@
 
 @bot.message_handler(commands=["audio", "aud"])
 @handler_formatter(text=True)
 def text_to_audio(message: telebot.types.Message):
     """Convert text to audio"""
     audio_chunk = audio_generator.text_to_audio(
         message=message.text,
-        voice=voice,
+        voice=User(message.chat.id).chat_voice,
         timeout=timeout,
     )
     return bot.send_audio(message.chat.id, audio=audio_chunk, caption=message.text)
 
 
 @bot.message_handler(commands=["reset"])
 @handler_formatter()
@@ -235,15 +328,15 @@
         ```
         """
 
     except Exception as e:
         response = f"ERROR : {e.args[1] if e.args and len(e.args)>1 else e}"
 
     finally:
-        return bot.send_message(message.chat.id, response)
+        return send_long_text(message, response)
 
 
 @bot.message_handler(content_types=["text"])
 @handler_formatter(text=True)
 def text_chat(message: telebot.types.Message):
     """Text generation"""
     user = User(message.from_user.id)
@@ -257,13 +350,13 @@
     ai_response = text_generator.AUTO(is_conversation=False, timeout=timeout).chat(
         conversation_prompt
     )
     conversation.update_chat_history(
         prompt=message.text, response=ai_response, force=True
     )
     user.update_history(conversation.chat_history)
-    return bot.send_message(message.chat.id, text=ai_response)
+    return send_long_text(message, ai_response)
 
 
 @bot.message_handler(func=lambda val: True)
 def any_other_action(message):
     return bot.reply_to(message, home.__doc__)
```

### Comparing `pytgpt_bot-0.0.5/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.0.6/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -30,15 +30,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytelegrambotapi==4.17.0
 Requires-Dist: python-tgpt==0.6.6
 Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: appdirs==1.4.4
 Requires-Dist: click==8.1.3
 
 <p align="center">
 <a href="https://github.com/Simatwa/pytgpt-bot/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=MIT&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt"/></a>
 <a href="https://pypi.org/project/pytgpt-bot"><img alt="PyPi" src="https://img.shields.io/pypi/v/pytgpt-bot?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
@@ -47,15 +46,15 @@
 <a href="https://github.com/Simatwa/pytgpt-bot/releases"><img src="https://img.shields.io/github/v/release/Simatwa/pytgpt-bot?color=success&label=Release&logo=github" alt="Latest release"></img></a> 
 -->
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/pytgpt-bot"/></a>
 <a href="https://wakatime.com/badge/github/Simatwa/pytgpt-bot"><img src="https://wakatime.com/badge/github/Simatwa/pytgpt-bot.svg" alt="wakatime"></a>
 </p>
 
 <h1 align="center">
-Welcome to <a href="https://github.com/Simatwa/pytgpt-bot">pytgpt-bot</a>
+Welcome to <a href="https://t.me/pytgpt_bot">pytgpt-bot</a>
 </h1>
 
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/python-tgpt), a powerful tool designed to enhance your interactions with AI. This bot is built on the robust foundation of the `pyTelegramBotAPI` and offers a wide range of features to make your experience with AI more engaging and interactive. Whether you're looking to chat with AI, generate images and audio from text, `pytgpt-bot` has got you covered.
 
 ## Prerequisites
 
 - [x] [Python>=3.10](https://python.org)
@@ -86,81 +85,51 @@
 
 Alternatively, using CLI interface::
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
-### 1. Chat with AI
+### Commands
 
-- **Command**: `/chat`
-- **Description**: Engage in a conversation with AI. This feature allows you to interact with the bot in a natural, conversational manner.
+- `/help`: This command displays the help information, providing users with a list of available commands and a brief description of what each command does. It's a useful way for users to quickly understand how to interact with the bot.
 
-### 2. Generate Images from Text
+- `/chat`: Allows users to engage in natural language conversations with the AI. This command initiates a chat session where users can ask questions, make requests, or simply chat with the AI.
 
-- **Command**: `/image`
-- **Description**: Generate images from text descriptions. This feature uses AI to create visual representations of your text inputs, making it a fun and creative way to explore the capabilities of AI.
+- `/image`: This command is used to generate images from text descriptions. Users can input a text description, and the bot will attempt to create an image based on that description. This feature can be particularly useful for visualizing ideas or concepts.
 
-- **Variant**: `/prodia`
-- **Description**: Generate images from text descriptions using the Prodia AI model. This variant offers a different style of image generation, providing a unique twist to your creative endeavors.
+- `/prodia`: Similar to `/image`, this command also generates images from text descriptions. However, it uses a different provider (Prodia) to create the images. This could offer a different style or interpretation of the text descriptions compared to the default method.
 
-### 3. Generate Audio from Text
+- `/audio`: Converts text to speech. Users can input text, and the bot will generate an audio file that reads out the text. This can be useful for listening to descriptions, instructions, or any text content.
 
-- **Command**: `/audio`
-- **Description**: Generate audio from text. This feature allows you to convert your text inputs into spoken words, enabling you to listen to the AI's voice or use the audio for other purposes.
+- `/sintro`: Allows users to set a new text for the chat intro. This can be used to customize the greeting message that users see when they start a new chat session with the bot.
 
-### 4. Check Current Chat Introduction
+- `/svoice`: Lets users set a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
 
-- **Command**: `/intro`
-- **Description**: Check the current chat introduction. This feature allows you to view the introduction text set for the current chat, providing context and setting the tone for your interactions.
+- `/awesome`: Sets an awesome prompt as the introductory message for the chat. This could be a motivational quote, a fun fact, or any other type of prompt that might inspire or engage users in their interactions with the bot.
 
-### 5. Check Chat History
+- `/history`: Checks the chat history. This command allows users to view the history of their chats with the bot. It can be useful for users who want to review past interactions or find specific information from previous conversations.
 
-- **Command**: `/history`
-- **Description**: Check the chat history. This feature allows you to review past interactions within the chat, helping you to recall previous discussions and decisions.
+- `/settings`: Checks the current settings of the bot. This command provides users with an overview of the bot's current configuration, including any custom settings they have applied.
 
-### 6. Set New Value for Chat Introduction
+- `/reset`: Starts a new chat thread. This command resets the chat history and starts a new conversation thread. It's useful for users who want to start fresh or who want to clear their chat history for privacy reasons.
 
-- **Command**: `/sintro`
-- **Description**: Set a new value for the chat introduction. This feature enables you to customize the introduction text for the current chat, allowing you to tailor the conversation to your preferences.
+- `/myid`: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for any reason, such as setting up bot admin.
 
-### 7. Start New Chat Thread
+- `/default`: Chat with AI. This command is essentially an alias for `/chat`, allowing users to initiate a chat session with the AI using a different command.
 
-- **Command**: `/reset`
-- **Description**: Start a new chat thread. This feature allows you to begin a fresh conversation with the bot, resetting the chat history and allowing for a new start.
+### Administrative Commands
 
-### 8. Echo Your Telegram ID
+- `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
 
-- **Command**: `/myid`
-- **Description**: Echo your Telegram ID. This feature provides you with your unique Telegram ID, useful for personalized interactions or for troubleshooting purposes and configuring admin.
+- `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
 
-### 9. Clear chat data
+- `/drop`: Clears the entire chat table. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data.
 
-- **Command**: `/clear_chats`
-- **Description**: This is an administrative command for deleting all entries of chat database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 10. Check total Chat
-
-- **Command**: `/total_chats`
-- **Description**: This is an administrative command for checking total chat records. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 11. Drop entire chat
-
-- **Command**: `/drop_chats`
-- **Description**: This is an administrative command that **drops** entire chat table and create new one. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 12. Run sql statements
-
-- **Command**: `/sql`
-- **Description**: This is an administrative command for running **SQL STATEMENTS** against the database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-
-### 12. Default Chat with AI
-
-- **Command**: `<Any other text>`
-- **Description**: Engage in a default chat with AI. This command is a shortcut to the `/chat` command, offering a quick and straightforward way to start a conversation with the bot.
+- `/sql`: Allows running SQL statements against the database. This command provides a way for administrators to directly interact with the bot's database using SQL queries. It's a powerful tool for managing and analyzing the bot's data but should be used with caution to avoid unintended data loss or corruption.
 
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.5 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.6 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -17,15 +17,15 @@
 Python Modules Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pytelegrambotapi==4.17.0 Requires-Dist: python-tgpt==0.6.6 Requires-Dist:
-python-dotenv==1.0.0 Requires-Dist: appdirs==1.4.4 Requires-Dist: click==8.1.3
+python-dotenv==1.0.0 Requires-Dist: click==8.1.3
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/
    _a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_g_p_t_-_b_o_t_]
                                   _[_w_a_k_a_t_i_m_e_]
                       ************ WWeellccoommee ttoo _pp_yy_tt_gg_pp_tt_--_bb_oo_tt ************
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/
 python-tgpt), a powerful tool designed to enhance your interactions with AI.
 This bot is built on the robust foundation of the `pyTelegramBotAPI` and offers
@@ -36,61 +36,61 @@
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the server
 `python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
-Features ### 1. Chat with AI - **Command**: `/chat` - **Description**: Engage
-in a conversation with AI. This feature allows you to interact with the bot in
-a natural, conversational manner. ### 2. Generate Images from Text -
-**Command**: `/image` - **Description**: Generate images from text
-descriptions. This feature uses AI to create visual representations of your
-text inputs, making it a fun and creative way to explore the capabilities of
-AI. - **Variant**: `/prodia` - **Description**: Generate images from text
-descriptions using the Prodia AI model. This variant offers a different style
-of image generation, providing a unique twist to your creative endeavors. ###
-3. Generate Audio from Text - **Command**: `/audio` - **Description**: Generate
-audio from text. This feature allows you to convert your text inputs into
-spoken words, enabling you to listen to the AI's voice or use the audio for
-other purposes. ### 4. Check Current Chat Introduction - **Command**: `/intro`
-- **Description**: Check the current chat introduction. This feature allows you
-to view the introduction text set for the current chat, providing context and
-setting the tone for your interactions. ### 5. Check Chat History -
-**Command**: `/history` - **Description**: Check the chat history. This feature
-allows you to review past interactions within the chat, helping you to recall
-previous discussions and decisions. ### 6. Set New Value for Chat Introduction
-- **Command**: `/sintro` - **Description**: Set a new value for the chat
-introduction. This feature enables you to customize the introduction text for
-the current chat, allowing you to tailor the conversation to your preferences.
-### 7. Start New Chat Thread - **Command**: `/reset` - **Description**: Start a
-new chat thread. This feature allows you to begin a fresh conversation with the
-bot, resetting the chat history and allowing for a new start. ### 8. Echo Your
-Telegram ID - **Command**: `/myid` - **Description**: Echo your Telegram ID.
-This feature provides you with your unique Telegram ID, useful for personalized
-interactions or for troubleshooting purposes and configuring admin. ### 9.
-Clear chat data - **Command**: `/clear_chats` - **Description**: This is an
-administrative command for deleting all entries of chat database. The user's
-Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
-pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-### 10. Check total Chat - **Command**: `/total_chats` - **Description**: This
-is an administrative command for checking total chat records. The user's
-Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
-pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-### 11. Drop entire chat - **Command**: `/drop_chats` - **Description**: This
-is an administrative command that **drops** entire chat table and create new
-one. The user's Telegram ID must match the one set at the [.env](https://
-github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/
-env#L2) config file. ### 12. Run sql statements - **Command**: `/sql` -
-**Description**: This is an administrative command for running **SQL
-STATEMENTS** against the database. The user's Telegram ID must match the one
-set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/
-7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file. ### 12. Default
-Chat with AI - **Command**: `` - **Description**: Engage in a default chat with
-AI. This command is a shortcut to the `/chat` command, offering a quick and
-straightforward way to start a conversation with the bot. ## Support and
-Feedback If you have any questions, feedback, or suggestions for `pytgpt`,
-please feel free to reach out. Your input is valuable in helping us improve and
-expand the bot's capabilities. ## License `pytgpt-bot` is open-source and
-available under the [MIT License](LICENSE). Feel free to use, modify, and
-distribute the code as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy
-your AI-powered interactions!
+Features ### Commands - `/help`: This command displays the help information,
+providing users with a list of available commands and a brief description of
+what each command does. It's a useful way for users to quickly understand how
+to interact with the bot. - `/chat`: Allows users to engage in natural language
+conversations with the AI. This command initiates a chat session where users
+can ask questions, make requests, or simply chat with the AI. - `/image`: This
+command is used to generate images from text descriptions. Users can input a
+text description, and the bot will attempt to create an image based on that
+description. This feature can be particularly useful for visualizing ideas or
+concepts. - `/prodia`: Similar to `/image`, this command also generates images
+from text descriptions. However, it uses a different provider (Prodia) to
+create the images. This could offer a different style or interpretation of the
+text descriptions compared to the default method. - `/audio`: Converts text to
+speech. Users can input text, and the bot will generate an audio file that
+reads out the text. This can be useful for listening to descriptions,
+instructions, or any text content. - `/sintro`: Allows users to set a new text
+for the chat intro. This can be used to customize the greeting message that
+users see when they start a new chat session with the bot. - `/svoice`: Lets
+users set a new voice for speech synthesis. This command enables users to
+choose from different voices for the AI to use when generating audio from text.
+- `/awesome`: Sets an awesome prompt as the introductory message for the chat.
+This could be a motivational quote, a fun fact, or any other type of prompt
+that might inspire or engage users in their interactions with the bot. - `/
+history`: Checks the chat history. This command allows users to view the
+history of their chats with the bot. It can be useful for users who want to
+review past interactions or find specific information from previous
+conversations. - `/settings`: Checks the current settings of the bot. This
+command provides users with an overview of the bot's current configuration,
+including any custom settings they have applied. - `/reset`: Starts a new chat
+thread. This command resets the chat history and starts a new conversation
+thread. It's useful for users who want to start fresh or who want to clear
+their chat history for privacy reasons. - `/myid`: Echoes the user's Telegram
+ID. This command is useful for users who need to know their Telegram ID for any
+reason, such as setting up bot admin. - `/default`: Chat with AI. This command
+is essentially an alias for `/chat`, allowing users to initiate a chat session
+with the AI using a different command. ### Administrative Commands - `/clear`:
+Clears all chats. This command is used to remove all chat data from the bot's
+database. It's a powerful command that should be used with caution, as it will
+delete all chat history. - `/total`: Shows the total number of chats available.
+This command provides an overview of the current chat data stored in the bot's
+database, helping administrators understand the volume of interactions the bot
+has had. - `/drop`: Clears the entire chat table. Similar to `/clear`, this
+command removes all data from the chat table in the database. It's a more
+drastic measure than `/clear`, as it completely wipes out all chat data. - `/
+sql`: Allows running SQL statements against the database. This command provides
+a way for administrators to directly interact with the bot's database using SQL
+queries. It's a powerful tool for managing and analyzing the bot's data but
+should be used with caution to avoid unintended data loss or corruption. ##
+Support and Feedback If you have any questions, feedback, or suggestions for
+`pytgpt`, please feel free to reach out. Your input is valuable in helping us
+improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
+source and available under the [MIT License](LICENSE). Feel free to use,
+modify, and distribute the code as you see fit. --- Thank you for using
+`pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.0.5/setup.py` & `pytgpt_bot-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.0.5",
+    version="0.0.6",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Telegram bot for text generation, text-to-image and text-to-audio conversions.",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
@@ -33,15 +33,14 @@
             "pytgpt-bot = pytgpt_bot.cli:entry",
         ],
     },
     install_requires=[
         "pytelegrambotapi==4.17.0",
         "python-tgpt==0.6.6",
         "python-dotenv==1.0.0",
-        "appdirs==1.4.4",
         "click==8.1.3",
     ],
     python_requires=">=3.10",
     keywords=[
         "ai",
         "tgpt",
         "pytgpt",
```

