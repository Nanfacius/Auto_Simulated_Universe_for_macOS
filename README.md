# Auto_Simulated_Universe
星穹铁道-模拟宇宙自动化-mocOS版

使用指南：

1 - 使用PlayCover运行iPadOS版崩坏星穹铁道。

2.- 设置键盘映射，可以从 https://github.com/PlayCover/keymaps 下载

3 - 修改macOS系统分辨率大于1920x1080，修改游戏分辨率为1920 x 1080。注意PlayCover中设置的游戏分辨率不等于逻辑分辨率，可以用计算器计算出需要的分辨率。例如，在macbook pro 14寸屏幕下，设置游戏分辨率为2494 x 1367，可以使逻辑分辨率恰好等于1920 x 1080。如果游戏闪退报错，可以通过重新签名解决，方法为打开终端，输入 sudo codesign -f -d -s - 游戏安装位置（或把.app文件图标拖进来）

4 - 安装Python依赖库：打开终端，cd 到本项目路径，输入 pip install -r requirements.txt

5 - 运行程序：打开终端，输入python states.py,

效果展示：https://www.bilibili.com/video/BV1Pb4y157U3/