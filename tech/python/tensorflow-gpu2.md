root@DataLX01:~# pip install --upgrade https://storage.googleapis.com/tensorflow/linux/gpu/tensorflow_gpu-1.7.0-cp36-cp36m-linux_x86_64.whl
~~~
Looking in indexes: http://ftp.daumkakao.com/pypi/simple
Collecting tensorflow-gpu==1.7.0 from https://storage.googleapis.com/tensorflow/linux/gpu/tensorflow_gpu-1.7.0-cp36-cp36m-linux_x86_64.whl
  Downloading https://storage.googleapis.com/tensorflow/linux/gpu/tensorflow_gpu-1.7.0-cp36-cp36m-linux_x86_64.whl (256.2MB)
    100% |████████████████████████████████| 256.2MB 236kB/s 
Requirement not upgraded as not directly required: absl-py>=0.1.6 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu==1.7.0) (0.1.12)
Requirement not upgraded as not directly required: wheel>=0.26 in /usr/lib/python3/dist-packages (from tensorflow-gpu==1.7.0) (0.29.0)
Requirement not upgraded as not directly required: tensorboard<1.8.0,>=1.7.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu==1.7.0) (1.7.0)
Requirement not upgraded as not directly required: protobuf>=3.4.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu==1.7.0) (3.5.2.post1)
Requirement not upgraded as not directly required: termcolor>=1.1.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu==1.7.0) (1.1.0)
Requirement not upgraded as not directly required: astor>=0.6.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu==1.7.0) (0.6.2)
Requirement not upgraded as not directly required: numpy>=1.13.3 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu==1.7.0) (1.14.2)
Requirement not upgraded as not directly required: gast>=0.2.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu==1.7.0) (0.2.0)
Requirement not upgraded as not directly required: grpcio>=1.8.6 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu==1.7.0) (1.10.0)
Requirement not upgraded as not directly required: six>=1.10.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu==1.7.0) (1.11.0)
Requirement not upgraded as not directly required: html5lib==0.9999999 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.8.0,>=1.7.0->tensorflow-gpu==1.7.0) (0.9999999)
Requirement not upgraded as not directly required: werkzeug>=0.11.10 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.8.0,>=1.7.0->tensorflow-gpu==1.7.0) (0.14.1)
Requirement not upgraded as not directly required: markdown>=2.6.8 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.8.0,>=1.7.0->tensorflow-gpu==1.7.0) (2.6.11)
Requirement not upgraded as not directly required: bleach==1.5.0 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.8.0,>=1.7.0->tensorflow-gpu==1.7.0) (1.5.0)
Requirement not upgraded as not directly required: setuptools in /usr/local/lib/python3.6/dist-packages (from protobuf>=3.4.0->tensorflow-gpu==1.7.0) (39.0.1)
socketio 0.0.7 has requirement setuptools==3.3, but you'll have setuptools 39.0.1 which is incompatible.
Installing collected packages: tensorflow-gpu
  Found existing installation: tensorflow-gpu 1.7.0
    Uninstalling tensorflow-gpu-1.7.0:
      Successfully uninstalled tensorflow-gpu-1.7.0
Successfully installed tensorflow-gpu-1.7.0
~~~
root@DataLX01:~# ipython
~~~
Python 3.6.3 (default, Oct  6 2017, 08:44:35) 
Type 'copyright', 'credits' or 'license' for more information
IPython 6.2.1 -- An enhanced Interactive Python. Type '?' for help.

In [1]: import tensorflow as tf
/usr/local/lib/python3.6/dist-packages/h5py/__init__.py:36: FutureWarning: Conversion of the second argument of issubdtype from `float` to `np.floating` is deprecated. In future, it will be treated as `np.float64 == np.dtype(float).type`.
  from ._conv import register_converters as _register_converters

In [2]: hello = tf.constant('Hello, Tensorflow!')

In [3]: sess = tf.Session()
2018-04-20 22:28:17.454555: I tensorflow/core/platform/cpu_feature_guard.cc:140] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2 FMA
2018-04-20 22:28:17.493627: E tensorflow/stream_executor/cuda/cuda_driver.cc:406] failed call to cuInit: CUDA_ERROR_UNKNOWN
2018-04-20 22:28:17.493738: I tensorflow/stream_executor/cuda/cuda_diagnostics.cc:145] kernel driver does not appear to be running on this host (DataLX01): /proc/driver/nvidia/version does not exist

In [4]: print(sess.run(hello))
b'Hello, Tensorflow!'

In [5]: quit()
root@DataLX01:~# 
~~~~
