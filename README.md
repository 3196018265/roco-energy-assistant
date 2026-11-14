# Roco Energy Assistant

**简体中文 / English UI · Windows x64 · v0.10.0**

A floating desktop assistant for duo battles in Roco Kingdom. It detects the energy button and sends X or a mouse click. If your teammate leaves, it can flee and stop monitoring. Click **Start monitoring** manually when the next duo battle begins. Choose **English** in the top-right language menu; your selection is saved.

Download the ZIP from [Releases](https://github.com/3196018265/roco-energy-assistant/releases/latest), extract the entire folder, and open `游戏助手.exe`. The .NET runtime is included. Interception must be installed once, followed by a Windows restart. Read [QUICKSTART-EN.md](QUICKSTART-EN.md) for setup. Recognition templates currently target the Chinese game UI; selecting English changes this assistant's interface, not the game's language or image templates.

## 简介 / Overview

一个用于双人战斗的 Windows 屏幕助手。识别到聚能按钮后，自动按 X 或点击鼠标；开启“双人对战”后，队友中途离开时自动退出当前战斗，并停止监听。

**当前正式版本：0.10**（发布标签 `v0.10.0`）。

## 下载

前往 [最新正式版本](https://github.com/3196018265/roco-energy-assistant/releases/latest)，下载 `RocoEnergyAssistant-0.10.0-win-x64.zip`。请下载软件 ZIP，而不是 GitHub 自动生成的 `Source code`。

本仓库用于发布程序、使用说明和更新文件；自有程序源码暂不公开。第三方组件的源码及许可按相应要求随软件提供。

## 功能

- 悬浮窗口，可置顶、收起设置。
- 识别聚能图案，支持 X 按键或鼠标点击；能量数字变化不影响内置模板。
- 使用“开始监听”“暂停监听”按钮控制。
- 右上角切换简体中文 / English，语言选择自动保存。
- 双人对战中，队友离开后自动逃跑并停止监听；下一场需要手动点击“开始监听”。
- 队友离开后才开启监听，只剩第二个位置的自身状态栏时，也能确认离开并退出。
- 支持游戏窗口选择、设备选择、一次检测及自定义聚能模板。
- 正式包支持启动检查更新，提示并下载安装新版本；必要更新完成前无法开始监听。

## 第一次使用

1. 面向 Windows 10 / 11 64 位。先将 ZIP 完整解压，再打开 `游戏助手.exe`。本包自带 .NET 运行环境，无需 Python、OCR 或额外安装 .NET。
2. 首次需要 Interception 驱动：运行包内 `安装驱动.cmd`，确认管理员提示，安装成功后手动重启。已经安装并重启过的用户无需重复安装。
3. 打开游戏和助手，选择游戏窗口，确认驱动就绪。
4. 进入双人战斗，先点“仅检测一次”检查，再点“开始监听”。
5. 保持游戏在前台，移动助手，避开左上角状态栏、聚能按钮和退出弹窗。停止时点“暂停监听”。

驱动可能与部分系统或键鼠设备不兼容，请先测试。遇到安装或安全提示，先核实来源，不要关闭系统安全保护。详细说明见 [使用说明.md](使用说明.md)。

## 更新

打开助手时会联网检查版本，也可以在设置中点击“检查更新”。发现新版本后，确认下载安装；需要强制更新时，完成更新才能继续监听。更新会保留 `config` 中的设置和自定义模板，安装后重新打开助手，监听需要手动开启。

GitHub 无法访问或检查失败时，请先恢复网络再重试；也可以从 Releases 下载完整包。当前版本不包含收费激活、设备绑定或自动付款功能。

## 隐私与使用提示

截图识别在本机进行，没有截图上传或游戏账号密码采集功能。更新请求使用 GitHub 下载服务。

这是第三方辅助工具，与游戏官方无隶属关系。请自行确认游戏规则允许的范围；不承诺无封禁风险、所有设备兼容或操作必定成功。首次使用请在旁观察，不要仅根据“已发送操作”判断游戏已经响应。

## 第三方许可

输入实现参考 [Auto-Roco](https://github.com/yorusacri/Auto-rocokingdom)（MIT），使用 [Interception](https://github.com/oblitum/Interception) 官方未修改 DLL 和驱动，随包保留许可及对应源码。Interception 商业授权需单独核实；本项目不代表已获商业授权。第三方权利不受本项目自有代码条款限制。

反馈问题时请说明软件版本、Windows 版本、触发方式和现象，附上去除个人信息的截图即可。
