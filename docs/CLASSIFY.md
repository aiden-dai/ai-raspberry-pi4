# Image Classification 

Test image classfication using Tensorflow Lite. Make sure Tensorflow Lite interpreter is installed.

## Reference

This is the official example from Tensorflow Lite

https://github.com/tensorflow/examples/blob/master/lite/examples/image_classification/raspberry_pi/README.md

## Run

The pre-trained model and labels have been included. To run a test:

```bash
cd python
python3 image_classification.py
```

Example

<img src="../images/cat.png" width='50%'>

You need to connect to a monitor via HMDI in order to see the camera preview screen, if you are using VNC, you can go to 'VNC Server - Options' > Troubleshooting,  check the 'Enable direct capture model'

<img src="../images/vnc_option.png" width='50%'>