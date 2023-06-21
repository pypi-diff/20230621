# Comparing `tmp/ailingbot-0.0.1.tar.gz` & `tmp/ailingbot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailingbot-0.0.1.tar", max compression
+gzip compressed data, was "ailingbot-0.0.2.tar", max compression
```

## Comparing `ailingbot-0.0.1.tar` & `ailingbot-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.1/LICENSE
--rw-r--r--   0        0        0     7499 2023-06-19 10:33:02.568500 ailingbot-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.1/ailingbot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021690 ailingbot-0.0.1/ailingbot/brokers/__init__.py
--rw-r--r--   0        0        0     1966 2023-06-13 06:48:58.022336 ailingbot-0.0.1/ailingbot/brokers/broker.py
--rw-r--r--   0        0        0     4985 2023-06-13 06:48:58.022939 ailingbot-0.0.1/ailingbot/brokers/pika_broker.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.1/ailingbot/channels/__init__.py
--rw-r--r--   0        0        0     3758 2023-06-19 06:33:23.090036 ailingbot-0.0.1/ailingbot/channels/channel.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.1/ailingbot/channels/dingtalk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.1/ailingbot/channels/feishu/__init__.py
--rw-r--r--   0        0        0     5142 2023-06-19 06:23:15.297803 ailingbot-0.0.1/ailingbot/channels/feishu/agent.py
--rw-r--r--   0        0        0      736 2023-06-19 04:32:16.486131 ailingbot-0.0.1/ailingbot/channels/feishu/render.py
--rw-r--r--   0        0        0     4617 2023-06-19 10:03:29.683603 ailingbot-0.0.1/ailingbot/channels/feishu/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.1/ailingbot/channels/slack/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.1/ailingbot/channels/wechatwork/__init__.py
--rw-r--r--   0        0        0     4383 2023-06-19 04:21:54.734917 ailingbot-0.0.1/ailingbot/channels/wechatwork/agent.py
--rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.1/ailingbot/channels/wechatwork/encrypt.py
--rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.1/ailingbot/channels/wechatwork/render.py
--rw-r--r--   0        0        0     5076 2023-06-14 09:09:34.335986 ailingbot-0.0.1/ailingbot/channels/wechatwork/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.1/ailingbot/chat/__init__.py
--rw-r--r--   0        0        0     4397 2023-06-14 09:09:34.336394 ailingbot-0.0.1/ailingbot/chat/chatbot.py
--rw-r--r--   0        0        0     3353 2023-06-19 04:12:03.268708 ailingbot-0.0.1/ailingbot/chat/messages.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.1/ailingbot/chat/policies/__init__.py
--rw-r--r--   0        0        0     1557 2023-06-19 06:33:23.067488 ailingbot-0.0.1/ailingbot/chat/policies/echo.py
--rw-r--r--   0        0        0     2386 2023-06-18 13:01:00.192045 ailingbot-0.0.1/ailingbot/chat/policies/langchain.py
--rw-r--r--   0        0        0     1801 2023-06-18 13:01:00.169542 ailingbot-0.0.1/ailingbot/chat/policy.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.1/ailingbot/cli/__init__.py
--rw-r--r--   0        0        0    17093 2023-06-19 10:08:05.721553 ailingbot-0.0.1/ailingbot/cli/cli.py
--rw-r--r--   0        0        0     4293 2023-06-18 13:01:00.235801 ailingbot-0.0.1/ailingbot/cli/options.py
--rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.1/ailingbot/cli/render.py
--rw-r--r--   0        0        0     1599 2023-06-19 06:33:23.048320 ailingbot-0.0.1/ailingbot/cli/setting.py
--rw-r--r--   0        0        0     1509 2023-06-15 05:43:12.897597 ailingbot-0.0.1/ailingbot/config.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.1/ailingbot/endpoint/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033407 ailingbot-0.0.1/ailingbot/repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033650 ailingbot-0.0.1/ailingbot/repositories/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.1/ailingbot/shared/__init__.py
--rw-r--r--   0        0        0     3953 2023-06-13 06:48:58.034885 ailingbot-0.0.1/ailingbot/shared/abc.py
--rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.1/ailingbot/shared/errors.py
--rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.1/ailingbot/shared/misc.py
--rw-r--r--   0        0        0     1048 2023-06-19 10:28:46.246819 ailingbot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8936 1970-01-01 00:00:00.000000 ailingbot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6347 2023-06-21 10:56:08.852892 ailingbot-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.2/ailingbot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021690 ailingbot-0.0.2/ailingbot/brokers/__init__.py
+-rw-r--r--   0        0        0     1940 2023-06-21 04:05:07.363931 ailingbot-0.0.2/ailingbot/brokers/broker.py
+-rw-r--r--   0        0        0     4642 2023-06-21 04:29:08.996776 ailingbot-0.0.2/ailingbot/brokers/pika_broker.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.2/ailingbot/channels/__init__.py
+-rw-r--r--   0        0        0     3643 2023-06-21 08:27:09.822487 ailingbot-0.0.2/ailingbot/channels/channel.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.2/ailingbot/channels/dingtalk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.2/ailingbot/channels/feishu/__init__.py
+-rw-r--r--   0        0        0     5120 2023-06-21 04:20:13.833468 ailingbot-0.0.2/ailingbot/channels/feishu/agent.py
+-rw-r--r--   0        0        0      736 2023-06-19 04:32:16.486131 ailingbot-0.0.2/ailingbot/channels/feishu/render.py
+-rw-r--r--   0        0        0     4580 2023-06-21 04:20:13.827390 ailingbot-0.0.2/ailingbot/channels/feishu/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.2/ailingbot/channels/slack/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.2/ailingbot/channels/wechatwork/__init__.py
+-rw-r--r--   0        0        0     4350 2023-06-21 04:14:09.084365 ailingbot-0.0.2/ailingbot/channels/wechatwork/agent.py
+-rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.2/ailingbot/channels/wechatwork/encrypt.py
+-rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.2/ailingbot/channels/wechatwork/render.py
+-rw-r--r--   0        0        0     5050 2023-06-21 04:20:13.825716 ailingbot-0.0.2/ailingbot/channels/wechatwork/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.2/ailingbot/chat/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-21 08:26:56.359421 ailingbot-0.0.2/ailingbot/chat/chatbot.py
+-rw-r--r--   0        0        0     3353 2023-06-19 04:12:03.268708 ailingbot-0.0.2/ailingbot/chat/messages.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.2/ailingbot/chat/policies/__init__.py
+-rw-r--r--   0        0        0     1550 2023-06-21 04:13:29.677392 ailingbot-0.0.2/ailingbot/chat/policies/echo.py
+-rw-r--r--   0        0        0     2390 2023-06-21 04:13:29.695901 ailingbot-0.0.2/ailingbot/chat/policies/langchain.py
+-rw-r--r--   0        0        0     1761 2023-06-21 04:13:29.672032 ailingbot-0.0.2/ailingbot/chat/policy.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.2/ailingbot/cli/__init__.py
+-rw-r--r--   0        0        0    12635 2023-06-21 04:30:47.588258 ailingbot-0.0.2/ailingbot/cli/cli.py
+-rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.2/ailingbot/cli/options.py
+-rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.2/ailingbot/cli/render.py
+-rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.2/ailingbot/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.2/ailingbot/endpoint/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033407 ailingbot-0.0.2/ailingbot/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033650 ailingbot-0.0.2/ailingbot/repositories/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.2/ailingbot/shared/__init__.py
+-rw-r--r--   0        0        0     3953 2023-06-13 06:48:58.034885 ailingbot-0.0.2/ailingbot/shared/abc.py
+-rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.2/ailingbot/shared/errors.py
+-rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.2/ailingbot/shared/misc.py
+-rw-r--r--   0        0        0     1068 2023-06-21 10:56:30.338610 ailingbot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7826 1970-01-01 00:00:00.000000 ailingbot-0.0.2/PKG-INFO
```

### Comparing `ailingbot-0.0.1/LICENSE` & `ailingbot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.1/README.md` & `ailingbot-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,218 +2,162 @@
 
 ---
 
 ![Python package workflow](https://github.com/ericzhang-cn/ailingbot/actions/workflows/python-package.yml/badge.svg)
 ![Pylint workflow](https://github.com/ericzhang-cn/ailingbot/actions/workflows/pylint.yml/badge.svg)
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
 
-<img src="./img/logo.png" alt="logo" width="50" height="50"/>
+<img src="https://github.com/ericzhang-cn/ailingbot/raw/main/img/logo.png" alt="logo" width="50" height="50"/>
 
-AilingBot - An all-in-one solution to empower your IM bot with AI.
+AilingBot - An all-in-one solution to empower your IM bot with LLM.
 
 # Features
 
-- 💯**Open source&Free**: Completely open source and free.
-- 📦**Out of the box**: No development is required, with pre-built capabilities to integrate with mainstream IM and LLM
-  models.
-- 🔗**Integrated LangChain**: The ability to integrate LangChain allows for the direct use of LangChain's pre-existing
-  chains or agents.
-- 🧩**Modular**: The project is organized in a modular way, with modules depending on abstract protocols, and similar
-  modules
-  implementing the protocols for plug-and-play functionality.
-- 💻**Extensible**: It can expand the usage scenarios and capabilities of AilingBot. For example, integrating with new
-  instant messaging platforms, new language learning models, or developing their own chains, agents, and chat policy.
-- 🚀**High Performance**: AilingBot uses coroutine-based asynchronous mode to improve the system's high-concurrency
-  performance. Meanwhile, the core servers can start multiple processes to further improve the system's high-concurrency
-  processing capabilities.
-- 🔌**Integrating through API**: AilingBot provides a set of clear API interfaces, which facilitates integration and
-  collaboration with other systems and processes.
+- 💯**Open source & free**: Completely open source and free
+- 📦**Out-of-the-box**: No development required, pre-installed with the ability to integrate with existing mainstream IM
+  and LLM models
+- 🔗**Integrated with LangChain**: Integrated with LangChain's ability to directly use pre-installed Chains or Agents
+- 🧩**Modular**: The project is organized in a modular way, with modules depending on abstract protocols between them.
+  Similar modules can implement protocols and be used immediately
+- 💻**Scalable**: AilingBot's usage scenarios and capabilities can be expanded. For example, integrating with new IM, new
+  LLM, or developing your own Chain, Agent, and chat policy
+- 🚀**High performance**: AilingBot uses coroutine-based asynchronous mode to improve system's high concurrency
+  performance. At the same time, the core process can start multiple processes to further improve the system's high
+  concurrency processing capability
+- 🔌**Integrated through API**: AilingBot provides a set of clear API interfaces for easy integration and collaboration
+  with other systems and processes
 
-# IM support list
+# List of supported IMs
 
 ## Supported
 
-- WeChat Work
+- Enterprise WeChat
 - Feishu
 
 ## Coming soon
 
 - DingTalk
 - Slack
 
-# Quickstart Guide
+# Quick Start Guide
 
-## Launch an AI Chatbot in 5 Minutes
+## Start an AI chatbot in 5 minutes
 
-### Installation
+Below you will see how to quickly start a command-line-based AI chatbot through AilingBot, with the effect as shown in
+the figure:
+![Command-line robot](https://github.com/ericzhang-cn/ailingbot/raw/main/img/command-line-screenshot.png)
+
+
+> 💡First, you need an OpenAI API key. If you don't have one, apply here: https://platform.openai.com/account/api-keys
+
+### Through Docker
 
 ```shell
-pip install ailingbot
+git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
+cd ailingbot
+docker build -t ailingbot .
+docker run -it --rm -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={Your OpenAI API key} ailingbot poetry run ailingbot bot chat
 ```
 
-- You also need an OpenAI API key. If you don't have one, please apply for it
-  here: https://platform.openai.com/account/api-keys
+### Through PIP
 
-### Initialize Configuration File
+#### Installation
 
 ```shell
-ailingbot init --silence
+pip install ailingbot
 ```
 
-This will create a file named settings.toml in the current directory,
-which is the configuration file for AilingBot. Next, modify the necessary configurations.
-To start the bot, you only need to configure one item.
-Find the following section in settings.toml:
+#### Generate configuration file
+
+```shell
+ailingbot init --silence --overwrite
+```
+
+At this point, a file called settings.toml will be created in the current directory, which is AilingBot's configuration
+file.
+Next, modify the necessary configurations. To start the robot, only one configuration is required. Find the following
+section in settings.toml:
 
 ```toml
-[policy.args.lc_chain_config.llm]
+[policy.llm]
 _type = "openai"
 model_name = "gpt-3.5-turbo"
-openai_api_key = "Your OpenAI API key"
+openai_api_key = ""
 temperature = 0
 ```
 
-Change the value of `openai_api_key` to your actual OpenAI API key.
+Change the value of `openai_api_key` to your real OpenAI API key.
 
-### Start the Bot
+#### Start the robot
 
-Start the bot with the following command:
+Start the robot with the following command:
 
 ```shell
-ailingbot bot chat -c settings.toml
+ailingbot bot chat
 ```
 
-You can now have a conversation with the bot through an interactive dialogue environment, as shown below:
-![Command-Line Screenshot](img/command-line-screenshot.png)
-
-## Connect to Instant Messaging Tools
-
-Below we take WeChat Work as an example to demonstrate how AilingBot can be quickly connected to instant messaging
-tools.
+## Integrating Instant Messaging Tools
 
-### Prerequisites
+Here's how to quickly integrate the above robot into Enterprise WeChat.
 
-To connect to WeChat Work, in addition to the prerequisites above, you also need to install the following environment:
+### Through Docker
 
-- RabbitMQ: https://www.rabbitmq.com/
+```shell
+export AILINGBOT_CHANNEL__AGENTID={Your Enterprise WeChat application AgentId}
+export AILINGBOT_CHANNEL__CORPSECRET={Your Enterprise WeChat application CorpSecret}
+export AILINGBOT_CHANNEL__AES_KEY={Your Enterprise WeChat application Webhook AES Key}
+export AILINGBOT_CHANNEL__CORPID={Your Enterprise WeChat application CorpId}
+export AILINGBOT_CHANNEL__TOKEN={Your Enterprise WeChat application Webhook Token}
+export AILINGBOT_POLICY__LLM__OPENAI_API_KEY={Your OpenAI API key}
+docker compose up
+```
 
-- Assumes you already have a usable WeChat Work app and are familiar with the WeChat Work app development process. If
-  you're not familiar with this, please refer to the WeChat Work official developer
-  documentation: https://developer.work.weixin.qq.com/
+### Through PIP
 
-### Modify the configuration file.
+#### Modify the configuration file
 
-Open settings.toml, the complete content is as follows:
+Open `settings.toml` and fill in the following section with your Enterprise WeChat application's real information:
 
 ```toml
-# This is the AilingBot configuration file template. Please modify it as needed.
-
-lang = "zh_CN"
-tz = "Asia/Shanghai"
-
-[broker]
-name = "pika"
-
-[broker.args]
-host = "localhost"
-port = 5672
-user = ""
-password = ""
-timeout = 5
-queue_name_prefix = ""
-
-[policy]
-name = "lc_conversation_chain"
-
-[policy.args]
-
-[policy.args.lc_chain_config.llm]
-_type = "openai"
-model_name = "gpt-3.5-turbo"
-openai_api_key = "Your OpenAI API key"
-temperature = 0
-
 [channel]
-
-[channel.agent]
 name = "wechatwork"
-
-[channel.agent.args]
-corpid = "WechatWork corpid"
-corpsecret = "WechatWork corpsecret"
+corpid = ""
+corpsecret = ""
 agentid = 0
-
-[channel.webhook]
-name = "wechatwork"
-
-[channel.webhook.args]
-token = "WechatWork webhook token"
-aes_key = "WechatWork webhook aes_key"
-
-[channel.uvicorn.args]
-host = "0.0.0.0"
-port = 8080
+token = ""
+aes_key = ""
 ```
 
-Here are the places that need to be filled in as needed:
-
-- `openai_api_key = "Your OpenAI API key"`
-- `corpid = "WechatWork corpid"`
-- `corpsecret = "WechatWork corpsecret"`
-- `agentid = 0`
-- `token = "WechatWork webhook token"`
-- `aes_key = "WechatWork webhook aes_key"`
-
-### Start the Bot
-
-To connect to instant messaging tools, three commands need to be executed to start the corresponding processes
-separately:
-
-Start the Channel Webhook process. The purpose of this process is to receive messages sent by users to the WeChat Work
-app as a webhook:
-
-```shell
-ailingbot channel serve_webhook -c settings.toml
-```
-
-Start the Bot Serve process. The purpose of this process is to listen for user messages received via the webhook and
-generate reply messages based on the corresponding chat policy:
+#### Start the service
 
 ```shell
-ailingbot bot serve -c settings.toml
+ailingbot bot serve
+ailingbot bot channel serve_agent
+ailingbot bot channel serve_webhook
 ```
 
-Start the Channel Agent process. The purpose of this process is to send the reply messages generated by the Bot Serve
-process to the user:
-
-```shell
-ailingbot channel serve_agent -c settings.toml
-```
-
-### Configure Webhook
-
-Finally, we need to go to the WeChat Work management console to configure the webhook address so that WeChat Work knows
-to forward the received user messages to our webhook.
-The webhook URL is: `http(s)://your_public_IP:8080/webhook/wechatwork/event/`
+Finally, we need to go to the Enterprise WeChat management console to configure the webhook address so that Enterprise
+WeChat knows to forward the received user messages to our webhook.
+The URL of the webhook is: `http(s)://your_public_IP:8080/webhook/wechatwork/event/`
 
-After completing the above configuration, you can find the bot in WeChat Work and start a conversation:
+After completing the above configuration, you can find the robot in Enterprise WeChat and start a conversation:
 
-<img src="./img/wechatwork-screenshot.png" alt="WeChat Work Bot" width="400"/>
+<img src="https://github.com/ericzhang-cn/ailingbot/raw/main/img/wechatwork-screenshot.png" alt="Enterprise WeChat robot" width="400"/>
 
-# Roadmap
+# Development Plan
 
-- [ ] Provide comprehensive user and developer documentation.
-- [ ] Support more IM platforms, such as DingTalk and Slack.
-- [ ] Support more commonly used LLM prompting paradigms and out-of-the-box chat policy.
-- [ ] Provide support for commonly used capabilities in LLM Chain, such as Vector Embedding&Query and Grounding.
-- [ ] Provide a WebUI.
-- [ ] Provide one-click deployment capability based on Docker containers.
-- [ ] Enhance the system's observability and manageability.
+- [ ] Provide complete usage and developer documentation
+- [ ] Support more IM clients, such as DingTalk, Slack, etc.
+- [ ] Support more commonly used LLM prompting paradigms and out-of-the-box chat policy
+- [ ] Provide support for common capabilities in LLM Chain, such as Vector Embedding&Query and Grounding
+- [ ] Provide a WebUI
+- [ ] Provide one-click deployment capability based on Docker containers
+- [ ] Enhance system observability and govern
 
-# License
+# 许可协议
 
 > MIT License
 >
 >Copyright (c) 2023 AilingBot
 >
 >Permission is hereby granted, free of charge, to any person obtaining a copy
 > of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ailingbot-0.0.1/ailingbot/brokers/broker.py` & `ailingbot-0.0.2/ailingbot/brokers/broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,23 +46,23 @@
 
         :return: Response message.
         :rtype: ResponseMessage
         """
         raise NotImplementedError
 
     @staticmethod
-    def get_broker(name: str, **kwargs) -> MessageBroker:
+    def get_broker(name: str) -> MessageBroker:
         """Gets broker instance.
 
         :param name: Built-in broker name or full path of broker class.
         :type name: str
         :return: Broker instance.
         :rtype: MessageBroker
         """
         if name.lower() == 'pika':
             from ailingbot.brokers.pika_broker import PikaMessageBroker
 
-            instance = PikaMessageBroker(**kwargs)
+            instance = PikaMessageBroker()
         else:
-            instance = get_class_dynamically(name)(**kwargs)
+            instance = get_class_dynamically(name)()
 
         return instance
```

### Comparing `ailingbot-0.0.1/ailingbot/brokers/pika_broker.py` & `ailingbot-0.0.2/ailingbot/brokers/pika_broker.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,68 +6,49 @@
 
 import aio_pika
 from loguru import logger
 
 import ailingbot.shared.errors
 from ailingbot.brokers.broker import MessageBroker
 from ailingbot.chat.messages import ResponseMessage, RequestMessage
+from ailingbot.config import settings
 
 
 class PikaMessageBroker(MessageBroker):
     """Pika message broker.
 
     Using Pika(AMQP protocol) as message broker.
     """
 
-    def __init__(
-        self,
-        *,
-        host: str = 'localhost',
-        port: int = 5672,
-        user: str = '',
-        password: str = '',
-        timeout: int = 5,
-        queue_name_prefix: str = '',
-    ):
-        """Creates instance.
-
-        :param host: AMQP host.
-        :type host: str
-        :param port: AMQP port.
-        :type port: int
-        :param user: AMQP user.
-        :type user: str
-        :param password: AMQP password.
-        :type password: str
-        :param timeout: Timeout for consuming message.
-        :type timeout: int
-        :param queue_name_prefix: Prefix of queue name.
-        :type queue_name_prefix: str
-        """
+    def __init__(self):
+        """Creates instance."""
         super(PikaMessageBroker, self).__init__()
 
-        self.host = host
-        self.port = port
-        self.user = user
-        self.password = password
-        self.timeout = timeout
+        self.host = settings.broker.host or 'localhost'
+        self.port = settings.broker.port or 5672
+        self.user = settings.broker.user or ''
+        self.password = settings.broker.password or ''
+        self.timeout = settings.broker.timeout or 5
+        self.queue_name_prefix = settings.broker.queue_name_prefix or ''
         self.connection: typing.Optional[
             aio_pika.abc.AbstractConnection
         ] = None
         self.channel: typing.Optional[aio_pika.abc.AbstractChannel] = None
         self.exchange: typing.Optional[aio_pika.abc.AbstractExchange] = None
         self.req_queue: typing.Optional[aio_pika.abc.AbstractQueue] = None
         self.resp_queue: typing.Optional[aio_pika.abc.AbstractQueue] = None
 
         self.req_queue_name = 'ailingbot_request_queue'
         self.resp_queue_name = 'ailingbot_response_queue'
-        if queue_name_prefix != '':
-            self.req_queue_name = f'{queue_name_prefix}_{self.req_queue_name}'
+        if self.queue_name_prefix != '':
+            self.req_queue_name = (
+                f'{self.queue_name_prefix}_{self.req_queue_name}'
+            )
             self.resp_queue_name = (
-                f'{queue_name_prefix}_{self.resp_queue_name}'
+                f'{self.queue_name_prefix}_{self.resp_queue_name}'
             )
 
     async def _initialize(self) -> None:
         try:
             self.connection = await aio_pika.connect_robust(
                 f'amqp://{self.user}:{self.password}@{self.host}:{self.port}/',
                 timeout=5,
```

### Comparing `ailingbot-0.0.1/ailingbot/channels/channel.py` & `ailingbot-0.0.2/ailingbot/channels/channel.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,24 +31,22 @@
         :type message: ResponseMessage
         """
         raise NotImplementedError
 
     async def _startup(self) -> None:
         self.broker = MessageBroker.get_broker(
             settings.broker.name,
-            **settings.broker.args,
         )
         await self.broker.initialize()
 
     async def _main_task(self, *, number: int) -> None:
         try:
             response_message = await self.broker.consume_response()
             await self.send_message(response_message)
         except ailingbot.shared.errors.EmptyQueueError:
-            logger.info(f'Task{number}: No more response message to process.')
             await asyncio.sleep(1)
 
     async def _shutdown(self) -> None:
         await self.broker.finalize()
 
     @staticmethod
     def get_agent(name: str, num_of_tasks: int = 1) -> ChannelAgent:
```

### Comparing `ailingbot-0.0.1/ailingbot/channels/feishu/agent.py` & `ailingbot-0.0.2/ailingbot/channels/feishu/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         num_of_tasks: int = 1,
     ):
         """Initializes class."""
         super(FeishuAgent, self).__init__(
             num_of_tasks=num_of_tasks,
         )
 
-        self.app_id = settings.channel.agent.args.app_id
-        self.app_secret = settings.channel.agent.args.app_secret
+        self.app_id = settings.channel.app_id
+        self.app_secret = settings.channel.app_secret
         self.access_token: typing.Optional[str] = None
         self.expire_in: typing.Optional[arrow.Arrow] = None
 
     async def _get_access_token(self) -> str:
         """Gets Feishu API access token.
 
         Returns cached token if not expired, otherwise, refreshes token.
```

### Comparing `ailingbot-0.0.1/ailingbot/channels/feishu/render.py` & `ailingbot-0.0.2/ailingbot/channels/feishu/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.1/ailingbot/channels/feishu/webhook.py` & `ailingbot-0.0.2/ailingbot/channels/feishu/webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,15 @@
 
 class FeishuWebhookFactory(ChannelWebhookFactory):
     """Factory that creates Feishu webhook ASGI application."""
 
     def __init__(self):
         super(FeishuWebhookFactory, self).__init__()
 
-        self.verification_token = (
-            settings.channel.webhook.args.verification_token
-        )
+        self.verification_token = settings.channel.verification_token
 
         self.broker: typing.Optional[MessageBroker] = None
         self.app: typing.Optional[ASGIApplication | typing.Callable] = None
 
     async def create_webhook_app(self) -> ASGIApplication | typing.Callable:
         self.broker = MessageBroker.get_broker(settings.broker.name)
         self.app = FastAPI()
```

### Comparing `ailingbot-0.0.1/ailingbot/channels/wechatwork/agent.py` & `ailingbot-0.0.2/ailingbot/channels/wechatwork/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,17 @@
         num_of_tasks: int = 1,
     ):
         """Initializes class."""
         super(WechatworkAgent, self).__init__(
             num_of_tasks=num_of_tasks,
         )
 
-        self.corpid = settings.channel.agent.args.corpid
-        self.corpsecret = settings.channel.agent.args.corpsecret
-        self.agentid = settings.channel.agent.args.agentid
+        self.corpid = settings.channel.corpid
+        self.corpsecret = settings.channel.corpsecret
+        self.agentid = settings.channel.agentid
         self.access_token: typing.Optional[str] = None
         self.expire_in: typing.Optional[arrow.Arrow] = None
 
     async def _get_access_token(self) -> str:
         """Gets Wechatwork API access token.
 
         Returns cached token if not expired, otherwise, refreshes token.
```

### Comparing `ailingbot-0.0.1/ailingbot/channels/wechatwork/encrypt.py` & `ailingbot-0.0.2/ailingbot/channels/wechatwork/encrypt.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.1/ailingbot/channels/wechatwork/render.py` & `ailingbot-0.0.2/ailingbot/channels/wechatwork/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.1/ailingbot/channels/wechatwork/webhook.py` & `ailingbot-0.0.2/ailingbot/channels/wechatwork/webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 class WechatworkWebhookFactory(ChannelWebhookFactory):
     """Factory that creates wechatwork webhook ASGI application."""
 
     def __init__(self):
         super(WechatworkWebhookFactory, self).__init__()
 
-        self.token = settings.channel.webhook.args.token
-        self.aes_key = settings.channel.webhook.args.aes_key
+        self.token = settings.channel.token
+        self.aes_key = settings.channel.aes_key
 
         self.broker: typing.Optional[MessageBroker] = None
         self.app: typing.Optional[ASGIApplication | typing.Callable] = None
 
     async def create_webhook_app(self) -> ASGIApplication | typing.Callable:
         self.broker = MessageBroker.get_broker(settings.broker.name)
         self.app = FastAPI()
```

### Comparing `ailingbot-0.0.1/ailingbot/chat/chatbot.py` & `ailingbot-0.0.2/ailingbot/chat/chatbot.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,32 +76,27 @@
             response = await self.respond(
                 conversation_id=conversation_id, message=message
             )
             await self.broker.produce_response(response)
 
     async def _startup(self):
         if self.run_mode == BotRunMode.Broker:
-            self.broker = MessageBroker.get_broker(
-                settings.broker.name,
-                **settings.broker.args,
-            )
+            self.broker = MessageBroker.get_broker(name=settings.broker.name)
             await self.broker.initialize()
 
         self.policy = ChatPolicy.get_policy(
-            settings.policy.name,
+            name=settings.policy.name,
             debug=self.debug,
-            **settings.policy.args,
         )
         await self.policy.initialize()
 
     async def _main_task(self, *, number: int):
         try:
             request_message = await self.broker.consume_request()
         except ailingbot.shared.errors.EmptyQueueError:
-            logger.info(f'Task{number}: No more request message to process.')
             await asyncio.sleep(1)
             return
 
         conversation_id = request_message.sender_id
         if request_message.scope is not None:
             conversation_id = (
                 f'{conversation_id}-{request_message.scope.value}'
```

### Comparing `ailingbot-0.0.1/ailingbot/chat/messages.py` & `ailingbot-0.0.2/ailingbot/chat/messages.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.1/ailingbot/chat/policies/echo.py` & `ailingbot-0.0.2/ailingbot/chat/policies/echo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 import uuid
 
 from ailingbot.chat.messages import (
     RequestMessage,
     ResponseMessage,
     TextRequestMessage,
-    TextResponseMessage,
     FallbackResponseMessage,
     TabularResponseMessage,
 )
 from ailingbot.chat.policy import ChatPolicy
 
 
 class EchoChatPolicy(ChatPolicy):
     """Return message to the user with context, for testing purposes only."""
 
     def __init__(
         self,
         *,
         debug: bool = False,
+        **kwargs,
     ):
         super(EchoChatPolicy, self).__init__(debug=debug)
 
     async def respond(
         self, *, conversation_id: str, message: RequestMessage
     ) -> ResponseMessage:
         if not isinstance(message, TextRequestMessage):
```

### Comparing `ailingbot-0.0.1/ailingbot/chat/policies/langchain.py` & `ailingbot-0.0.2/ailingbot/chat/policies/langchain.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,35 +10,38 @@
     RequestMessage,
     ResponseMessage,
     TextRequestMessage,
     TextResponseMessage,
     FallbackResponseMessage,
 )
 from ailingbot.chat.policy import ChatPolicy
+from ailingbot.config import settings
 
 
 class LCChainChatPolicy(ChatPolicy):
     """Load LangChain chain and use the chain as chat policy"""
 
     def __init__(
         self,
         *,
         debug: bool = False,
-        lc_chain_config: dict,
     ):
         super(LCChainChatPolicy, self).__init__(debug=debug)
 
-        self.lc_chain_config = lc_chain_config
-
         self.chain: dict[str, Chain] = {}
 
     async def _load_chain(self) -> Chain:
+        config = {
+            '_type': settings.policy._type,
+            'llm': settings.policy.llm,
+            'prompt': settings.policy.prompt,
+        }
         if self.debug:
-            self.lc_chain_config['verbose'] = True
-        return load_chain_from_config(self.lc_chain_config)
+            config['verbose'] = True
+        return load_chain_from_config(config)
 
     async def respond(
         self, *, conversation_id: str, message: RequestMessage
     ) -> ResponseMessage:
         if not isinstance(message, TextRequestMessage):
             response = FallbackResponseMessage()
             response.reason = 'LCChainChatPolicy can only handle messages of type TextRequestMessage.'
@@ -58,18 +61,19 @@
 
 
 class LCConversationChain(LCChainChatPolicy):
     def __init__(
         self,
         *,
         debug: bool = False,
-        lc_chain_config: dict,
     ):
         super(LCConversationChain, self).__init__(
-            debug=debug, lc_chain_config=lc_chain_config
+            debug=debug,
         )
 
     async def _load_chain(self) -> Chain:
-        if self.debug:
-            self.lc_chain_config['verbose'] = True
-        llm = load_llm_from_config(self.lc_chain_config.get('llm', {}))
-        return ConversationChain(llm=llm, memory=ConversationBufferMemory())
+        llm = load_llm_from_config(settings.policy.llm)
+        return ConversationChain(
+            llm=llm,
+            memory=ConversationBufferMemory(),
+            verbose=self.debug,
+        )
```

### Comparing `ailingbot-0.0.1/ailingbot/chat/policy.py` & `ailingbot-0.0.2/ailingbot/chat/policy.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         :type conversation_id:
         :param message: Request message.
         :type message: RequestMessage
         """
         raise NotImplementedError
 
     @staticmethod
-    def get_policy(name: str, *, debug: bool = False, **kwargs) -> ChatPolicy:
+    def get_policy(name: str, *, debug: bool = False) -> ChatPolicy:
         """Gets policy instance.
 
         :param name: Built-in policy name or full path of policy class.
         :type name: str
         :param debug:
         :type debug:
         :return: Policy instance.
@@ -42,16 +42,16 @@
         if name.lower() == 'echo':
             from ailingbot.chat.policies.echo import EchoChatPolicy
 
             instance = EchoChatPolicy(debug=debug)
         elif name.lower() == 'lc_llm_chain':
             from ailingbot.chat.policies.langchain import LCChainChatPolicy
 
-            instance = LCChainChatPolicy(debug=debug, **kwargs)
+            instance = LCChainChatPolicy(debug=debug)
         elif name.lower() == 'lc_conversation_chain':
             from ailingbot.chat.policies.langchain import LCConversationChain
 
-            instance = LCConversationChain(debug=debug, **kwargs)
+            instance = LCConversationChain(debug=debug)
         else:
-            instance = get_class_dynamically(name)(debug=debug, **kwargs)
+            instance = get_class_dynamically(name)(debug=debug)
 
         return instance
```

### Comparing `ailingbot-0.0.1/ailingbot/cli/render.py` & `ailingbot-0.0.2/ailingbot/cli/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.1/ailingbot/config.py` & `ailingbot-0.0.2/ailingbot/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,9 +48,11 @@
     ),
 }
 
 # Settings entrypoint, loads settings from environment variables.
 settings = Dynaconf(
     envvar_prefix='AILINGBOT',
     load_dotenv=True,
-    settings_files=[],
+    settings_files=[
+        'settings.toml',
+    ],
 )
```

### Comparing `ailingbot-0.0.1/ailingbot/shared/abc.py` & `ailingbot-0.0.2/ailingbot/shared/abc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.1/ailingbot/shared/errors.py` & `ailingbot-0.0.2/ailingbot/shared/errors.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.1/ailingbot/shared/misc.py` & `ailingbot-0.0.2/ailingbot/shared/misc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.1/pyproject.toml` & `ailingbot-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ailingbot"
-version = "0.0.1"
+version = "0.0.2"
 description = "An all-in-one solution to empower your IM bot with LLM."
 authors = ["ericzhang-cn <ericzhang.buaa@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
@@ -26,14 +26,15 @@
 asgiref = "^3.5.2"
 tabulate = { version = "^0.9.0", extras = ["widechars"] }
 emoji = "^2.2.0"
 prompt-toolkit = "^3.0.33"
 langchain = "^0.0.192"
 openai = "^0.27.8"
 rich = "^13.4.2"
+tomlkit = "^0.11.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 sphinx = "^5.3.0"
 pytest-asyncio = "^0.20.1"
 blue = "^0.9.1"
```

