# B560M-AORUS-ELITE-OC

20211205更新

关闭核显图形输出（随航无图像输出）

调整DRM默认使用独显

调整USB错误端口

没有随航需求的小伙伴建议使用最新版


20211129更新

添加免驱蓝牙和Wi-Fi补丁（据说是12.0之后的版本机制变化）

修改核显ID为07009B3E，核显硬解开启，随航正常（测试设备iPad Pro2018）

添加启动参数，修复核显驱动后导致的开机速度慢及黑屏时间长

声卡由原先的启动参数改为注入ID（感觉没有爆破音了，可能是玄学）

注意事项，由于PC的核显通道为0,2,0,0，Mac核显通道为0,0,0,0所以DRM问题无解。导致问题：Apple Music无法播放无损音乐，Apple TV无法正常播放

       关于DRM临时解决方案：需要是可通过终端调用独显解码理论上只支持免驱卡
       
       开启独显：defaults write com.apple.AppleGVA gvaForceAMDKE -boolean yes
       
       启用核显：defaults write com.apple.AppleGVA gvaForceAMDKE -boolean no
       
故障：休眠第二次唤醒重启依然无解

硬件配置

主板技嘉： B560M AORUS ELITE

CPU： i5-10400（UHD630）

硬盘：三星970EVOPlus

显卡：蓝宝石RX6600XT超白金

内存：海盗船16*2 3600

网卡：BCM943602CS

硬件不同者请注意切换驱动文件

系统版本

引导：OPENCORE7.6

系统：macOS12.1beta3+win11

兼容状况

正常运行：USB内建，蓝牙正常，休眠正常，核显加速正常

已知问题：无法解决集显输出，无法解决开机黑屏3秒（主板集显芯片导致），第二次手动睡眠会导致重启（解决方案关闭睡眠，也是由集显导致）

20211123更新支持Apple DRM （具体验证方式可查看Apple Music是否可以播放无损音乐）。修改主板厂商为Apple Inc.，对苹果二合一卡的蓝牙适配更加友好，开机就可以连接自家的键盘和鼠标

       注意事项
       
       机箱前面板无USB-C接口的进系统后将HS03和SS03修改为USB2.0及USB3.0
       
       自行修改序列号并保存
       
![image](https://user-images.githubusercontent.com/57509476/144055359-7ba7c6d5-16a2-4502-80d7-68daad9f52e0.png)

![image](https://user-images.githubusercontent.com/57509476/144055448-282c10e3-f78a-427b-a5b9-a36fcdf11597.png)

![image](https://user-images.githubusercontent.com/57509476/144055499-f83cbf91-e341-46d1-97d4-32ffbfb51a1f.png)

远景地址：https://bbs.pcbeta.com/viewthread-1912918-1-1.html
