# 你叉叉

1. 新增对 `Oracle AMD，Oracle ARM`全面支持. 可支持从 Ubuntu, Oracle Linux 等系统网络重装.
2. 更新 dd 镜像的基础系统版本.
3. 移除对外部 wget 的依赖.
4. 新增 `-port` 参数, 可更改默认SSH端口.
5. 更新 内置的网络参数计算 逻辑.
6. 更新 grub 配置文件定位逻辑, 可支持任意引导grub的系统.
7. 新增 `-cmd`, 可接受开机后只运行一次的命令(base64编码).
8. 新增对 AWS EC2 (ARM) 网络重装的支持.

**以下系统已通过测试(其他自测):**
*Debian: 9, 10, 11;*
*Ubuntu: 18.04, 20.04;*
*CentOS: 6.10;*


## 首先安装所需的软件根据自己本身对应的系统选择对应的命令即可。

ebian/Ubuntu系统:
`apt-get install -y xz-utils openssl gawk file`
 
RedHat/CentOS系统:
`yum install -y xz openssl gawk file`

如果报错，那么先运行下面命令

Debian/Ubuntu系统:
`apt-get update`
 
RedHat/CentOS系统:
`yum update`

一键
```
bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/nbxxo/d/d/d.sh') -d 10 -v 64 -p 2511052 -a 
```
国内 `bash <(wget --no-check-certificate -qO- 'https://ghproxy.com/https://raw.githubusercontent.com/nbxxo/d/d/d.sh') -d 11 -v 64 -p 2511052 -a --mirror 'http://mirrors.ustc.edu.cn/debian/'`

默认密码：root / `2511052`
Debian10修改root默认密码
passwd root
用于甲骨文 `-firmware`

手动

```
wget --no-check-certificate -qO InstallNET.sh 'https://raw.githubusercontent.com/nbxxo/d/d/d.sh' && chmod a+x d.sh
```

bash d.sh -d 11 -v 64 -p 2511052 -a

Debian -d `7 8 9 10 11`

ubuntu -u `12.04 14.04 16.04 18.04 20.04`

centos -c `6.10`

全自动：-a

系统位数：-v 32-64
