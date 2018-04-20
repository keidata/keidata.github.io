root@DataLX01:~# pip install keras
Looking in indexes: http://ftp.daumkakao.com/pypi/simple
Requirement already satisfied: keras in /usr/local/lib/python3.6/dist-packages (2.1.5)
Requirement already satisfied: numpy>=1.9.1 in /usr/local/lib/python3.6/dist-packages (from keras) (1.14.2)
Requirement already satisfied: scipy>=0.14 in /usr/lib/python3/dist-packages (from keras) (0.17.0)
Requirement already satisfied: pyyaml in /usr/local/lib/python3.6/dist-packages (from keras) (3.12)
Requirement already satisfied: six>=1.9.0 in /usr/local/lib/python3.6/dist-packages (from keras) (1.11.0)
ipython 6.2.1 has requirement setuptools>=18.5, but you'll have setuptools 3.3 which is incompatible.
root@DataLX01:~# pip install --upgrade setuptools
Looking in indexes: http://ftp.daumkakao.com/pypi/simple
Collecting setuptools
  Downloading http://mirror.kakao.com/pypi/packages/20/d7/04a0b689d3035143e2ff288f4b9ee4bf6ed80585cc121c90bfd85a1a8c2e/setuptools-39.0.1-py2.py3-none-any.whl (569kB)
    100% |████████████████████████████████| 573kB 12.3MB/s 
socketio 0.0.7 has requirement setuptools==3.3, but you'll have setuptools 39.0.1 which is incompatible.
Installing collected packages: setuptools
  Found existing installation: setuptools 3.3
    Uninstalling setuptools-3.3:
      Successfully uninstalled setuptools-3.3
Successfully installed setuptools-39.0.1
root@DataLX01:~# pip install keras
Looking in indexes: http://ftp.daumkakao.com/pypi/simple
Requirement already satisfied: keras in /usr/local/lib/python3.6/dist-packages (2.1.5)
Requirement already satisfied: scipy>=0.14 in /usr/lib/python3/dist-packages (from keras) (0.17.0)
Requirement already satisfied: numpy>=1.9.1 in /usr/local/lib/python3.6/dist-packages (from keras) (1.14.2)
Requirement already satisfied: six>=1.9.0 in /usr/local/lib/python3.6/dist-packages (from keras) (1.11.0)
Requirement already satisfied: pyyaml in /usr/local/lib/python3.6/dist-packages (from keras) (3.12)
socketio 0.0.7 has requirement setuptools==3.3, but you'll have setuptools 39.0.1 which is incompatible.
root@DataLX01:~# 
