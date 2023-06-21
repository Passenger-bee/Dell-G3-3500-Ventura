# Dell-G3-3500-Ventura

Hackintosh 

### 引导版本：~~OpenCore 0.8.6（正式版）~~

**最新版本：OpenCore 0.9.2（正式版）**

### MacOS系统版本：Ventura 13.3.1  （Ventura13.4可能会导致黑屏无法亮屏）



———2023.6.21更新———

更新日志：

1.加入自制OpenCore主题

2.硬件更换：屏幕更换为NE156QHM-NY1，2.5k分辨率/165Hz 但是mac下还是60Hz😭

3.Readme.md图片已更新最新版本

4.其他功能完善



———2023.6.15更新———

更新日志：

1.OpenCore引导升级至 0.9.2 版本

2.ACPI更新及完善以适配最新版本macOS Ventura

3.更换SmBios为MacBook Pro15,3 （15寸，更适合你🥰）



————自制OpenCore主题————

Config：默认隐藏多余项目；支持Ctrl+Enter设置默认启动项

太喜欢简约风了没办法🤷‍♂️

<img src="https://github.com/Passenger-bee/Dell-G3-3500-Ventura/blob/main/README.assets/%E9%BB%91%E8%89%B2%E4%B8%BB%E9%A2%98.png?raw=true" alt="CPU频率" style="zoom: 25%;" />

<img src="https://github.com/Passenger-bee/Dell-G3-3500-Ventura/blob/main/README.assets/%E9%BB%91%E8%89%B2%E4%B8%BB%E9%A2%98%202.png?raw=true" alt="CPU频率" style="zoom: 25%;" />



 以下是实现的功能：

##    **首先是最重要的几个硬件驱动：**

**Smbios**: 使用MacBook15,3机型

<img src="https://github.com/Passenger-bee/Dell-G3-3500-Ventura/blob/main/README.assets/%E6%A6%82%E8%A7%88.png?raw=true" alt="系统详情" style="zoom: 35%;" />

**CPU电源管理**：已加载原生电源管理，但是我禁用了睿频，频率一直在2.5Ghz 可以大幅降低cpu热量（2.5Ghz就够用）

（通过Turbo Boost Switcher Pro这个app禁用）

<img src="https://github.com/Passenger-bee/Dell-G3-3500/blob/main/README.assets/cpu%E9%A2%91%E7%8E%87.png?raw=true" alt="CPU频率" style="zoom: 45%;" />

**显卡（核显）UHD630**：核显加速，硬解完美支持，一般视频剪辑都没有问题，已禁用独显GTX1650Ti。

<img src="https://github.com/Passenger-bee/Dell-G3-3500-Ventura/blob/main/README.assets/%E6%98%BE%E5%8D%A1.png?raw=true" alt="图形卡-显示器" style="zoom:35%;" />

​                                       未知显示器终于显示正常了 

<img src="https://github.com/Passenger-bee/Dell-G3-3500-Ventura/blob/main/README.assets/%E6%98%BE%E7%A4%BA%E5%99%A8.png?raw=true" alt="显示器" style="zoom:35%;" />

​            

**声音**：内置扬声器正常使用，但是内置麦克风、3.5mm音频插口无法使用，另外开机Boom无法发声。

ALC id为21，其他的id声音太小（调最高也很小），这个正常多了，但是这个id随之带来的一个问题就是睡眠唤醒无声，通过添加CodecCommander.kext解决。

 一个解决方案是：连接蓝牙音响，使用蓝牙音箱上的麦克风。

<img src="https://github.com/Passenger-bee/Dell-G3-3500-Ventura/blob/main/README.assets/%E5%A3%B0%E9%9F%B3.png?raw=true" alt="输出音量" style="zoom:35%;" />

**网络；蓝牙**：更换为苹果原装网卡以后，wifi、以太网、隔空投送、接力、随航、用AppleWatch解锁🔓一切如白苹果一般丝滑。

<img src="https://github.com/Passenger-bee/Dell-G3-3500-Ventura/blob/main/README.assets/wi-fi.png?raw=true" alt="网络" style="zoom:35%;" />

<img src="https://github.com/Passenger-bee/Dell-G3-3500-Ventura/blob/main/README.assets/%E8%93%9D%E7%89%99.png?raw=true" alt="蓝牙" style="zoom:35%;" />

#### **然后是其他不太重要的琐碎项目：**

**USB端口**：已映射两个usb2.0、 一个usb3.0、一个Type-C口（没啥用删除这个端口了）。

**睡眠**：自动睡眠，唤醒敲两下键盘，AppleWatch解锁丝滑无比。

**背光**：👌

**触控板**：支持白苹果手势，但是pc的触控板手感体验跟trash一样。

**SD读卡器**：👌

**摄像头**：👌

**iMessage、FaceTime**：👌

**AppleID、AppleStore**：👌

**BootCamp**：可以从win启动到mac，相反mac也可以启动到win。

 

#### **没有驱动的总结为以下：**

~~1.HDMI~~

~~2.内置麦克风~~

~~3.耳机3.5mm接口~~

~~4.Type-C没有进行测试（不知道能否可以进行外接显示器使用）~~



#### 一些杂语：

默认没有添加intel网卡驱动，需自行添加！！！

默认没有添加intel网卡驱动，需自行添加！！！

默认没有添加intel网卡驱动，需自行添加！！！

​    祝大家有美好的一天，Good Luck To You Guys！

​    有问题可以问我🤗

 

