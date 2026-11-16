# Roco Energy Assistant 0.20

A Windows desktop battle assistant for solo and duo battles in Roco Kingdom.

## Setup

Download `RocoEnergyAssistant-0.20.0-win-x64.zip` from Releases and extract the entire folder. Run `游戏助手.exe`. Windows 10 / 11 x64 is supported; the .NET runtime is included. No Python or OCR installation is needed.

On first use, run `安装驱动.cmd`, then restart Windows. A working Interception installation does not need reinstalling. Choose English beside Start monitoring, select your game window and battle plan, then start monitoring. Settings collapse automatically. Keep the game in the foreground. Pause monitoring to stop.

## Battle plans

Solo and duo battles share the Battle page and all plans:

- 1–4: repeat the selected skill.
- 5: energy only.
- 6: skill with energy fallback; choose the skill in the extra dropdown.
- 7: custom sequence, including order, repeats, waits and enemy-HP conditions. Sequences reset each battle and loop while the battle continues.

The energy-fallback checkbox applies to every skill plan. Gathering energy does not skip the pending skill. Action intervals sample a fresh value between your minimum and maximum; equal values give a fixed interval.

Enable teammate-departure protection for duo battles. After confirmed departure the assistant flees, confirms and stops monitoring. Start monitoring manually for the next battle.

## Battle catching

Enable catching, set the HP threshold (10% by default), and choose a ball slot from 1–6. Catching takes priority: open the ball menu, select the ball, wait for confirmation, then confirm. Failed catches retry after battle controls or the ball menu returns.

The Field catch tab is temporarily hidden in 0.20 while bugs are fixed. Saved field mode returns to Battle; samples and parameters are preserved.

## Input and statistics

Choose Hotkeys or Mouse in monitoring settings. Hotkeys uses skills 1–4, energy X, catch W, ball slots 1–6 and Space confirmation. Mouse clicks the corresponding controls.

Sessions lasting at least one minute with at least one observed battle generate a summary on stopping: battles, elapsed time, confirmed catches, energy, skill and throw counts. Battle throws require consecutive detections of the Chinese throw banner. A stable return to the field then counts as success; returning to battle or the ball menu does not. Animation, black frames or missing HUD alone never confirm a catch. Missed evidence remains unconfirmed.

The app checks GitHub for updates and preserves your config folder. If updating manually, copy your old config folder into the extracted new package. Keep all runtime files, third-party libraries and licenses.

English changes the assistant UI only. Recognition templates target the Chinese game UI. Screenshots are processed locally. Live game responses and capture flows require supervised playtesting. See 开源说明.md and the included licenses and third-party sources.
