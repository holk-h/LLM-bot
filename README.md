# LLM-bot
一个使用大语言模型来 聊天 | 做事 | 搜索信息 | ... 的机器人，使用nonebotv2、gocq-http，支持QQ、Telegram等平台。目前使用的是openai的chatgpt。
 a bot using LLM to chat | take actions | search info | ...

---

效果：会模仿真人，在群聊中聊天吹水。
下一步计划：支持让语言模型调用相应的操作函数，进行撤回消息、戳一戳、踢人、操作数据库等操作。

---
使用教程：
- 首先请参考[nonebotv2的文档](https://nb2.baka.icu/docs/)。 
- 其次请参考[gocq-http](https://github.com/Mrs4s/go-cqhttp)。
- 首先，你需要按照nonebotv2的文档，安装好`nb-cli`。
- 接下来，使用`nb create`创建一个项目。
- 使用`nb plugin install nonebot_plugin_chatrecorder`安装聊天记录插件
- 下载相应的后端，如果你要使用QQ，请下载[gocq-http](https://github.com/Mrs4s/go-cqhttp/releases/tag/v1.0.1)
- 运行gocq可执行文件，并按照提示来操作。
- 把本项目中的`pyproject.toml`、`.env.*`放入你自己的机器人项目文件夹，并替换原来的文件。
- 把`llmbot/plugins/llm_operation`放入你的插件文件夹（插件相关操作请参阅nonebot文档）
- 运行`nb run`