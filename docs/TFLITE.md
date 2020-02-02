# Install Tensorflow Lite

Install Tensorflow Lite interpreter

> This interpreter-only package is a fraction the size of the full TensorFlow package and includes the bare minimum code required to run inferences with TensorFlow Lite—it includes only the tf.lite.Interpreter Python class. This small package is ideal when all you want to do is execute .tflite models and avoid wasting disk space with the large TensorFlow library.

## Reference

https://tensorflow.google.cn/lite/guide/python


## Install
Install Tensorflow Lite interpreter on Python 3.7

```bash
wget https://dl.google.com/coral/python/tflite_runtime-2.1.0-cp37-cp37m-linux_armv7l.whl
pip3 install tflite_runtime-2.1.0-cp37-cp37m-linux_armv7l.whl
```


## Verify

Run python3
```bash
python3 -c "import tflite_runtime.interpreter as tflite"
```

