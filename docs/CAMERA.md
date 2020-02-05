# Use CSI Camera

This page is only for the use of CSI camera.

## Enable Camera

Run
```
sudo raspi-config
```

Interfacing Options -> Camera Enable

Reboot

## Test Photo

```
raspistill --help
raspistill -v -o test.jpg
raspistill -o test.jpg -t 2000
```

## Test Video

```
raspivid --help
raspivid -o test.h264
raspivid -o test.h264 -t 10000
raspivid -o test.h264 -t 10000 -w 1280 -h 720
```


## Use picamera in Python

> Reference: https://picamera.readthedocs.io/en/release-1.13/index.html

By default, picamera is already installed, run `python3 -c "import picamera"` to verify. Create a test python file to run:

```python
from time import sleep
from picamera import PiCamera

camera = PiCamera()
camera.resolution = (1024, 768)
camera.start_preview()
# Camera warm-up time
sleep(2)
camera.capture('test.jpg')
```