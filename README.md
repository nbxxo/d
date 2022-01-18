# 你牛逼叉叉的

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
bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/2511052/Note/master/InstallNET.sh') -d 10 -v 64 -a -p 2511052 -firmware
```
国内 `--mirror 'http://mirrors.ustc.edu.cn/debian/'`

默认密码：root / `2511052`
Debian10修改root默认密码
passwd root
用于甲骨文 `-firmware`


手动

```wget --no-check-certificate -qO InstallNET.sh 'https://raw.githubusercontent.com/2511052/Note/master/InstallNET.sh' && chmod a+x InstallNET.sh```

bash InstallNET.sh -d 11 -v 64 -p 2511052 -a

Debian -d `7 8 9 10 11`

ubuntu -u `12.04 14.04 16.04 18.04 20.04`

centos -c `6.10`

预设密码：-p

全自动：-a

系统位数：-v 32-64
