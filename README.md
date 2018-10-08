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

  

