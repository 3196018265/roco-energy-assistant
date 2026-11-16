# Roco Energy Assistant

**简体中文 / English · Windows x64 · v0.20.0**

和好友牵手刷异色时，我经常作为第二位玩家反复聚能，帮助队友推进战斗。为了减少这些重复操作，做了这个桌面悬浮助手。0.20 将单人和双人合并为“战斗”，现在也能选择技能和自定义行动序列。

A floating desktop assistant originally built to automate repeated energy actions as the second player in duo battles. Version 0.20 adds shared solo/duo battle plans, skills and custom sequences, with Chinese and English interfaces.

## Download / 下载

前往 [Releases](https://github.com/3196018265/roco-energy-assistant/releases/latest)，下载 **RocoEnergyAssistant-0.20.0-win-x64.zip** 并完整解压，运行 `游戏助手.exe`。请下载附件中的软件 ZIP，无需下载 GitHub 自动生成的 Source code。

Windows 10 / 11 64 位，自带 .NET 运行环境，无需安装 Python 或 OCR。首次使用需运行 `安装驱动.cmd` 并重启 Windows，已安装且正常工作的用户无需重复安装。

Download the ZIP, extract the entire folder and run `游戏助手.exe`. Install Interception once using `安装驱动.cmd` and restart Windows. Select English beside Start monitoring. See [QUICKSTART-EN.md](QUICKSTART-EN.md).

## Features / 功能

- 单人 / 双人共用“战斗”页，支持重复技能 1–4、一直聚能、技能 + 聚能、自定义序列。
- 技能不可用时可先聚能，再继续原技能；动作序列每场重置，战斗未结束时循环。
- 操作间隔支持最小 / 最大值，每次随机取值。
- 双人队友离开后自动逃跑、确认并停止监听；下一场手动开启。
- 战斗内可按生命阈值优先捕捉，咕噜球位置下拉选择 1–6。
- 运行满一分钟且识别过至少一场战斗时生成总结，显示战斗、耗时和确认捕捉数。
- 支持快捷键 / 鼠标、窗口置顶、自动收起设置、中文 / English 和保留配置的版本更新。

**局外捕捉暂不开放：0.20 隐藏“局外捕捉”页签，相关问题修复后再提供。战斗内捕捉仍保留。**

Field catch is temporarily hidden while bugs are fixed. Battle catching remains available. Saved field mode switches to Battle, preserving samples and settings.

## Quick start / 使用

1. 完整解压软件包；首次安装驱动并重启。
2. 打开助手，选择游戏窗口。
3. 在“战斗”页选择行动方案、操作间隔和所需选项。
4. 进入战斗，点击“开始监听”，设置自动收起；保持游戏前台。
5. 点击“暂停监听”停止。语言菜单位于开始按钮右侧。

详细说明：[使用说明.md](使用说明.md)。当前识别模板适用于中文游戏画面，英文菜单仅切换助手界面。

## Updates / 更新

0.10 用户可在助手中点击“检查更新”，或下载完整 0.20 软件包并复制旧目录的 `config` 文件夹。更新后需手动开始监听。网络不可用时可从 Releases 手动下载。

仓库用于发布程序、说明及更新文件，自有程序源码暂不公开。第三方组件的许可和对应源码随软件提供。截图在本机处理。

## Credits / 致谢

输入实现参考 [Auto-Roco](https://github.com/yorusacri/Auto-rocokingdom)（MIT），使用 [Interception](https://github.com/oblitum/Interception) 官方库和驱动，许可及对应源码随包提供。详见软件包内的 `开源说明.md`。

本工具与游戏官方无隶属关系。使用前请确认游戏规则允许的范围，首次使用请在旁确认实际效果。反馈时请提供版本、触发方式、复现步骤和去除个人信息的截图。
