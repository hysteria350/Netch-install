# Windows 平台上 Netch 安装与配置指南

## **简介**

Netch 是一款运行在 Windows 系统上的开源游戏加速工具，简单易上手。也可以用于日常的网页浏览等。

Github 项目地址：[https://github.com/NetchX/Netch](https://github.com/NetchX/Netch)

## **下载安装**

*   点击[这里](https://github.com/netchx/netch/releases/tag/1.9.2)下载。
    

**请注意：**

此软件运行需要 **.NET Framework 5.0** 支持，非 Windows 10 系统可能需要[点此进行安装](https://aka.ms/dotnet/5.0/windowsdesktop-runtime-win-x64.exe)

## **快速上手**

下载压缩包后进行完整解压，并双击运行主程序 Netch.exe。

![Netch-1.png](https://i.loli.net/2019/11/13/CxgrK98wd6mRVL2.png)

先进行 [订阅购买](https://shortlink.20250812.xyz/1) ，获取到订阅链接。订阅链接位于：仪表盘 > 一键订阅 , 然后复制订阅地址或者扫描二维码订阅。

![Netch-2.png](https://i.loli.net/2019/11/13/ehfKiaL84ukEA19.png)

点击**订阅**，选择**管理订阅连接**。

![Netch-3.png](https://i.loli.net/2019/11/13/HRxjrN1Mly7FXsC.png)

在对应的地方粘贴自己的订阅链接，备注可以自行填写。点击**添加**后再点击**保存**。初次配置时不建议勾选左下角的选项。

![Netch-4.jpg](https://i.loli.net/2019/11/13/r1qoibPRxB4wJfH.jpg)

**添加订阅后，需要回到主界面选择更新订阅，将服务器信息同步到本地。**

![Netch-5.png](https://i.loli.net/2019/11/13/AM8DBpdUxZIym6L.png)

在节点列表选择一个节点。节点后方的数字为延迟。

![Netch-6.png](https://i.loli.net/2019/11/13/NKzSGxHgkADmP3Y.png)

选择自己需要的代理模式。这里推荐 `Bypass LAN and China` 或 `绕过局域网和中国大陆`，此模式下可以进行自动分流，不影响国内服务速度。

![Netch-7.png](https://i.loli.net/2019/11/13/2EWxGCdge7BOiUv.png)

点击**启动**。

此时您的电脑已经可以访问国际网络。

![Netch-8.png](https://i.loli.net/2019/11/13/GysfEFiBZSDMV3t.png)

![Netch-9.png](https://i.loli.net/2019/11/13/T2kQpZ5cGsnxzKi.png)

## **更多**

### **为自己的游戏添加进程代理**

如果你的游戏的模式已经被收录，也可以考虑在模式菜单中，选择使用已收录的模式。所有模式的文件，都在 `./mode/` 文件夹下，如果你需要多个模式的合并文件，可以使用记事本将其打开，将多个文件合并。

ping 值未必准确，因为这只是你本地到代理服务器而非游戏服务器的延迟。

如果你的游戏的模式没被收录，可以看接下来的扫描步骤来手动创建模式。

请点击菜单栏上的 **模式** ，然后点击 **创建进程模式**。

![Netch-10.png](https://i.loli.net/2019/11/13/WrMti1DQCbAyRad.png)

在弹出的窗口中点击扫描

![Netch-11.png](https://i.loli.net/2019/11/13/bzLQpIVW5JdDEiF.png)

选择你要加速的游戏的安装路径，根据游戏不同，可能需要选择多个不同的目录进行扫描。

由于编写教程时的电脑上没有安装游戏，故此处用 Chrome 浏览器来演示，原理是相同的。

![Netch-12.png](https://i.loli.net/2019/11/13/xSL9BYZzQ7XcmjN.png)

比如 Chrome 的安装根目录为 C:\\Program Files (x86)\\Google\\Chrome ，点击扫描可得

![Netch-13.png](https://i.loli.net/2019/11/13/QJ2iXvj5utFDBbc.png)

输入备注名后点击保存。

![Netch-14.png](https://i.loli.net/2019/11/13/ulkpo4x3FJKPGmS.png)

此时已经可以在代理模式窗口看到刚添加的进程模式了。

![Netch-15.png](https://i.loli.net/2019/11/13/lqGyHhL52cEP3UB.png)

*   启动 Netch 后，再去游戏根目录或者别的启动器如 Steam、Uplay 启动游戏即可。此时游戏就已经被代理了。
*   如果在 Netch 启动前就启动了游戏，建议重启游戏。
*   如果需要 Steam、Uplay 等启动器也被代理，参照前面的方式对 Steam、Uplay 根目录也进行扫描即可。
*   如果出现了启动失败，或者无法代理成功的情况，请先尝试 **选项** - **重启服务或选项** - **卸载服务**，或者在退出 Netch 以后，点击运行在 Netch 根目录下的 **DriverUpdater.exe** 程序进行驱动更新。
