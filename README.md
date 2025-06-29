## 在 Bandwagon 云服务器上使用 wulabing V2Ray 一键安装脚本

> 感谢 wulabing 提供的 V2Ray 一键安装脚本

> Thanks to wulabing for providing the V2Ray one-click installation script

### 操作系统选择

在 Bandwagon 的 KiwiVM 中，点击 Install new OS，选择 centos-8-x86_64，点击 Reload。

> 注意此处不能选择 centos-9-x86_64，否则后续执行安装脚本会报错。

![操作系统选择](https://github.com/yun-gif/Bandwagon-install-wulabing-V2Ray/blob/main/1.png)

### 脚本安装步骤

* 安装wget包
  
`yum install wget -y` 

> 此处不能执行`yum update -y` 更新服务器系统，否则后续执行安装脚本会报错。

![wget包安装](https://github.com/yun-gif/Bandwagon-install-wulabing-V2Ray/blob/main/2.png)

* 安装脚本（Vmess+websocket+TLS+Nginx+Website）

`wget -N --no-check-certificate -q -O install.sh "https://raw.githubusercontent.com/wulabing/V2Ray_ws-tls_bash_onekey/master/install.sh" && chmod +x install.sh && bash install.sh` 

![脚本安装](https://github.com/yun-gif/Bandwagon-install-wulabing-V2Ray/blob/main/3.png)

* 输入数字`1`

* 后面输入解析到 Bandwagon 云服务器 IP 的域名，一路回车即可。
