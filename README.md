# XiaoMi-GLP

- 9-17-2018
  - 添加网卡`Realtek 8111H/8168H`驱动
  - 更新显卡驱动方式
  - CLOVER常规更新
    - drivers64UEFI添加apfs.efi，以解决第二阶段安装找不到卷标的问题

- 10-8-2018 

  - 10.14.1破解`USB`端口限制补丁（去除限制）
  - disable IOBufferCopyController (Credit by DalianSky)，解决部分8代CPU无法全新安装的问题
  - 添加`USBPorts_XIAOMI_GLP.kext`，解决安装禁行以及睡眠唤醒问题
  - 添加`VoodooI2C`驱动，可能安装过程中会存在触摸板失效的问题，请通过`block injected kexts`禁用，安装成功后可正常使用
  - 添加`PM981`无法安装的驱动程序，**个人建议：PM981请直接绕行**
  - `CLOVER`常规更新到v4695

- 10-10-2018

  - 修改安装配置文件
    - `config_first.plist` 安装镜像第一阶段时使用，可能存在黑屏现象
    - `config_second.plist` 安装镜像第二、第三阶段使用
    - `config.plist` 安装完成后使用
  - `Whatevergreen` 更新到v1.2.4

- 10-17-2018

  - 八代核显亮屏的正确姿势：
    - 移除`SSDT-PNLF.aml`
    - 重新编译`WhateverGreen`，支持直接亮屏
    - 修改`config_installer.plist`和`config.plist`，增加亮屏参数
    - 添加`AppleBacklightInjector.kext`中对八代核显亮度的支持

  

  

# QQ群：

765888601 [小米游戏笔记本黑苹果](http://shang.qq.com/wpa/qunwpa?idkey=bef269b994e3738b66684b7c8821bd3390220552af9ab7d331f2f78487815f72) 

756750452 [小米游戏本吃黑果讨论](http://qm.qq.com/cgi-bin/qm/qr?k=6-mc7yVIzkdv-XTj9_HL8wKi5y74lgXE) 







