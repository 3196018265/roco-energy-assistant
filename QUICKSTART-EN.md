# Roco Energy Assistant 0.10

For duo battles in Roco Kingdom. The assistant detects the energy icon and sends X or a mouse click. If your teammate leaves, duo mode can flee the battle and stop monitoring. Start monitoring manually when the next duo battle begins.

1. Extract the complete ZIP to a regular folder. Run `游戏助手.exe` and accept the Windows administrator prompt. Do not move the EXE out of its folder. The .NET runtime is included; Python and OCR are not needed.
2. Interception is required. If it is not installed, run `安装驱动.cmd`, accept the administrator prompt, and restart Windows after a successful installation. Do not install it again if it is already installed and working. The script does not restart Windows automatically. Driver compatibility varies by system and device.
3. Select **English** in the top-right menu. Your language selection is saved. You can change languages while monitoring without resetting your settings.
4. Choose the game window. Under **Input devices**, check that the driver is ready. Leave both devices on **Automatic (recommended)** initially.
5. Enter a duo battle and use **Detect once** to test recognition. This check sends no input. Select **X key** or **Mouse click**, then click **Start monitoring**.
6. Keep the game in the foreground. Move the floating window away from the ally panels, energy button and flee confirmation dialog. Click **Pause monitoring** to stop.

If recognition fails, use **Select energy icon** and select only the icon, excluding the numbers and X. Press Esc to cancel selection. If the game ignores input, pause and try another input device or method.

If you start monitoring after your teammate has already left, duo mode can also flee when only your own ally panel remains in the second position. Monitoring stops after leaving; start it manually for the next duo battle.

The English option translates this assistant's interface. The bundled image templates currently target the Chinese game UI, including its flee confirmation. It does not add recognition for an English game client.

The release supports signed updates when its GitHub update source is configured. Configured releases require an online update check before monitoring; required updates must be installed to continue. Settings and custom templates are preserved. The local pre-release review build hides the update section until the publisher configures it.

Screenshots are processed locally. The assistant does not upload screenshots or collect game passwords; update checks connect to GitHub. This is an unofficial tool, not affiliated with the game. Check the game's rules before use; no compatibility or account-safety guarantee is made. Observe initial tests yourself.

Interception and other dependencies retain their own licenses; see `开源说明.md`, `许可证` and `第三方源码`. Commercial use of Interception requires checking the author's commercial licensing terms. Paid activation and device binding are not included.
