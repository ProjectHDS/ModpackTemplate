# ModpackTemplate

[简体中文版README](https://github.com/ProjectHDS/ModpackTemplate/blob/master/README.md).

Modpack template repository with all the action work files goodies, **DOES NOT ACCEPT ANY ISSUES OR FEATURE REQUIRES**.

For ''forge-1.12.2-14.23.5.2860'' only, but feel free to change it if you like.

The whole thing was deprecated from [Herodotus](https://github.com/ProjectHDS/Herodotus), some features had been removed in this template, go to the [Herodotus](https://github.com/ProjectHDS/Herodotus) for more.

Contains:
* gitignore whitelist, but only a standard setup.
* Versioner, automatically verions some files with action run numbers.
* FTBQuestsLangProcessor, automatically localizes all the [FTBQuests](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-forge) files
* Gitee Versioning, automatically updates a version JSON in a Gitee repository, using with [Versioner](https://www.curseforge.com/minecraft/mc-mods/versioner)
* CurseforgeDownloader, downloads mods from CurseForge, for independently using and AutoBuild.
* TestRunner, runs your pack with [Go Minecraft Launcher](https://github.com/xmdhs/gomclauncher), exit if the modpack is basically functional.
* AutoBuild, automatically builds server pack and curse format client pack and upload them to action artifacts with every push.
* AutoRelease/Tag, automatically build and release client/server pack when triggered.
* Simple Issues/PR Templates, some basic templates.

Everything above needs to be carefully configured, don't enable actions or use them in your main repositories before you have figured out **everything**.

Secrets:
* ACTION_TOKEN, for FTBQuestsLangProcessor commit and AutoRelease/Tag.
* GITEE_SSH_HOST, for Gitee Versioning push.
* GITEE_SSH_KEY, for Gitee Versioning push.
* OVERWOLF_API_KEY, for downloading mods.
