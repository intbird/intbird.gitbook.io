---
description: nexus 5 (root)
---

# FRPS

下载文件

{% embed url="https://github.com/fatedier/frp/releases/tag/v0.34.1" caption="frp\_0.34.1\_linux\_arm.tar.gz" %}

修改配置

> /Users/intbird/Downloads/frp\_0.34.1\_linux\_arm/frps.ini

> /Users/intbird/Downloads/frp\_0.34.1\_linux\_arm/frpc.ini

传输文件

> adb push /Users/intbird/Downloads/frp\_0.34.1\_linux\_arm /sdcard/

创建目录

> adb shell & su

> mkdir /data/user/frp/
>
> mv /sdcard/frp\_0.34.1\_linux\_arm   /data/user/frp/

添加授权

> cd /data/user/frp/frp\_0.34.1\_linux\_arm
>
> chmod 777 ./\*
>
> 运行软件

> ./frps -c ./frps.ini 
>
>  nohup ./frps -c ./frps.ini &gt;frp\_log.log 2&gt;&1 &

![](../.gitbook/assets/image%20%281%29.png)

