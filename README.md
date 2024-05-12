# Auto_Simulated_Universe_for_macOS
星穹铁道-模拟宇宙自动化-macOS版

使用指南：

1 - 使用PlayCover运行iPadOS版崩坏星穹铁道。

2.- 设置键盘映射，可以从 https://github.com/PlayCover/keymaps 下载

3 - 修改macOS系统分辨率大于1920 x 1080，修改游戏分辨率为1920 x 1080。注意PlayCover中设置的游戏分辨率不等于逻辑分辨率，可以用计算器计算出需要的分辨率。例如，在macbook pro 14寸屏幕下，设置游戏分辨率为2494 x 1367，可以使游戏窗口的逻辑分辨率恰好等于1920 x 1080。如果游戏闪退报错，可以通过重新签名解决，方法为打开终端，输入 `sudo codesign -f -d -s - 游戏安装位置（或把.app文件图标拖进来）`

4 - 安装Python依赖库：打开终端，cd 到本项目路径，输入 `pip install -r requirements.txt`

5 - 校准视角转动角度：`python align_angle.py` 如果角度仍不准确，可以多次校准

6 - 配队：建议1号位使用远程角色，把秘技立即进入战斗的角色放在靠后位置。若1号位为黄泉则默认使用秘技进入战斗，但不建议把黄泉放在1号位，因为容易卡墙角

7 - 运行程序：`python states.py`

8 - 退出程序：切换到终端窗口，按下Control + C。

可选功能：

1 - 绘制地图：当提示地图匹配度低，疑似在黑塔办公室，或移动方向明显错误时，可手动绘制地图。进入地图，输入`python states.py -find=0`，开启希儿、花火等隐身秘技，走到终点后，切换到终端，按下control + c退出程序。打开.\imgs\maps\ ，按添加日期排序，打开第一个地图文件夹，打开target.jpg，手动标点，用红色圆点标记怪物，黄色圆点标记终点，蓝色圆点标记途经点，保存。

2 - 获取奖励：`python states.py -bonus=1` 仅当沉浸器不为0时生效

效果展示：https://www.bilibili.com/video/BV1Pb4y157U3/

Honkai: Star Rail Auto Simulated Universe for macOS

Quick Guidence

1 - Run Honkai: Star Rail ipadOS version on PlayCover.

2 - Set keymapping. You can download keymap from https://github.com/PlayCover/keymaps

3 - Revise macOS resolution to more than 1920 x 1080 and revise the game resolution to 1920 x 1080. Notice that the resolution set by PlayCover is not necessariily equal to the logical resolution. You can use calculator to calculate the resolution needed. For example, if you use Macbook Pro with a 14 inch screen, set the game resolution to 2494 x 1367, then the logic resolution will be exactly 1920 x 1080. Besides, if the game crashes, you may solve the problem by re-signing. Open Terminal and type `sudo codesign -f -d -s - GameInstallationLocation.app (or drag the .app file)`

4 - Install Python dependencies: `cd ThisProjectDirectory`, then `pip install -r -requirements.txt`

5 - Align the viewing angle: `python align_angle.py`. If the angle is still inaccurate, align it for multiple times.

6 - Set the team: recommend setting a remote character as the first one. If Acheron is the first character, technique will be the default method to enter battles. However, it is not recommended to do so, in case that sometimes characters might be stuck in a corner.

7 - Run the program: `python states.py`

8 - Exit the program: Switch to the Terminal window and press control + C.

Options:

1 - Draw maps: when the program prints 地图匹配度低，疑似在黑塔办公室 (the matching score of the map is low) or when the moving direction is wrong, you may draw maps manually. Input `python states.py -find=0`, use Seele's or Sparkle's technique, walk to the exit and switch to the Terminal window, press control + C to exit. Then open .\imgs\maps\ and sort the files by date added. Open target.jpg in the first folder. Mark points with circles: red for enemies, yellow for exit and blue for passing points. Save the image.

2 - Acquire immersion reward: `python states.py -bonus=1`. This will happen only when the number of immersifiers is positive.

Notice: This project is designed for Chinese game interface only. You may change the language into Chinese before running it. 

Video display: https://www.bilibili.com/video/BV1Pb4y157U3/