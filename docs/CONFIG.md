# Basic Configuration


## Update Source

```
sudo vi /etc/apt/sources.list
```

Content as below:
```
deb http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ stretch main contrib non-free rpi

deb-src http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ stretch main contrib non-free rpi
```

```bash
sudo vi /etc/apt/sources.list.d/raspi.list
```
Content as below:
```
deb http://mirror.tuna.tsinghua.edu.cn/raspberrypi/ stretch main ui

deb-src http://mirror.tuna.tsinghua.edu.cn/raspberrypi/ stretch main ui
```
Then update
```
sudo apt-get update
```