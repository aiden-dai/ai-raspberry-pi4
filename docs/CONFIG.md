# Basic Configuration


## Update Sources List

- Run `sudo vi /etc/apt/sources.list`

Content as below:
```
deb http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ buster main non-free contrib
deb-src http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ buster main non-free contrib
```

- Run `sudo vi /etc/apt/sources.list.d/raspi.list`

Content as below:
```
deb http://mirrors.tuna.tsinghua.edu.cn/raspberrypi/ buster main ui
```

- Get updates

Run bash
```
sudo apt-get update
sudo apt-get upgrade
```

