# ModpackTemplate

[English verison of README](https://github.com/ProjectHDS/ModpackTemplate/blob/master/README_EN_US.md).

包含大量实用工具和工作流文件的整合包模板仓库，**不接受任何议题或特性请求**。

为 ''forge-1.12.2-14.23.5.2860'' 设计，可凭自身需要修改。

所有文件均从 [Herodotus](https://github.com/ProjectHDS/Herodotus) 分解，部分特性在此模板中已被移除，欲了解更多请查看 [Herodotus](https://github.com/ProjectHDS/Herodotus) 仓库。

包含：
* gitignore whitelist，基础配置版 gitignore 白名单。
* Versioner，自动根据 Action run number 对部分文件进行版本号修改。
* FTBQuestsLangProcessor，自动本地化所有 [FTBQuests](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-forge) 文件。
* Gitee Versioning，自动更新一个 Gitee 仓库中的版本信息JSON，需配合 [Versioner](https://www.curseforge.com/minecraft/mc-mods/versioner) 使用。
* CurseforgeDownloader，从 CurseForge 下载模组。
* TestRunner，使用 [Go Minecraft Launcher](https://github.com/xmdhs/gomclauncher) 运行整合包，可检查启动失败问题。
* AutoBuild，每次推送后自动构建 Curse 格式客户端或服务端，并上传至 Action Artifacts。
* AutoRelease/Tag，触发时自动应用标签和发布 Release。
* Simple Issues/PR Templates，简单的议题/拉取请求模板，双语。

以上所有功能均需配置，在能理解**所有东西**前，请不要启用 Actions 或在主仓库中使用。

需要配置的秘密：
* ACTION_TOKEN，FTBQuestsLangProcessor 提交和 AutoRelease/Tag 使用。
* GITEE_SSH_HOST，Gitee Versioning 推送使用。
* GITEE_SSH_KEY，Gitee Versioning 推送使用。
* OVERWOLF_API_KEY，下载模组使用。
