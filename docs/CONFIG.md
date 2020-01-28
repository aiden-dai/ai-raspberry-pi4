# Basic Configuration


## Update Sources List

- Run `sudo vi /etc/apt/sources.list`

Content as below:
```
deb http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ stretch main contrib non-free rpi

deb-src http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ stretch main contrib non-free rpi
```

- Run `sudo vi /etc/apt/sources.list.d/raspi.list`

Content as below:
```
deb http://mirror.tuna.tsinghua.edu.cn/raspberrypi/ stretch main ui

deb-src http://mirror.tuna.tsinghua.edu.cn/raspberrypi/ stretch main ui
```

- Get updates

Run bash
```
sudo apt-get update
sudo apt-get upgrade
```


## Update pip source

Create a file `～/.pip/pip.conf`, content as below
```
[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple

[install]
trusted-host = https://pypi.tuna.tsinghua.edu.cn
```