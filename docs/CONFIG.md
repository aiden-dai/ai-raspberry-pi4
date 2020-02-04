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
sudo apt update
sudo apt upgrade
```


## Enable VNC

To enable VNC, run

```
sudo raspi-config
```
Select Interfacing Options > VNC > Yes

Wait until you see 'The VNC Server is enabled'

<img src="../images/vnc.PNG" width='50%'>

Then change the resolution: Select Advanced Options > A5 Resolution

Reboot

Run `ifconfig` via ssh or `ping -4 raspberrypi.local` to check the ip address of Raspberry Pi, then connect to Raspberry Pi via VNC Viewer.

<img src="../images/vnc2.PNG" width='50%'>


## Enable Remote Desktop

To enable remote desktop connection (from Windows), run

```
sudo apt install xrdp
```

Open a connection, login with pi

<img src="../images/remote.PNG" width='50%'>

Login successfully.

<img src="../images/remote2.PNG" width='50%'>

> You can run `sudo service xrdp status` to check the status