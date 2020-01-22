# Use Camera

Test and use Camera

## Enable Camera


Run
```
sudo raspi-config
```

Interfacing Options -> Camera Enable

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