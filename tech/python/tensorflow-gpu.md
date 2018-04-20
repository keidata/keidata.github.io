https://www.tensorflow.org/install/install_linux

root@DataLX01:~# pip install tensorflow-gpu
~~~
Looking in indexes: http://ftp.daumkakao.com/pypi/simple
Requirement already satisfied: tensorflow-gpu in /usr/local/lib/python3.6/dist-packages (1.6.0)
Requirement already satisfied: grpcio>=1.8.6 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.10.0)
Requirement already satisfied: tensorboard<1.7.0,>=1.6.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.6.0)
Requirement already satisfied: numpy>=1.13.3 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.14.2)
Requirement already satisfied: astor>=0.6.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (0.6.2)
Requirement already satisfied: termcolor>=1.1.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.1.0)
Requirement already satisfied: wheel>=0.26 in /usr/lib/python3/dist-packages (from tensorflow-gpu) (0.29.0)
Requirement already satisfied: six>=1.10.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (1.11.0)
Requirement already satisfied: protobuf>=3.4.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (3.5.2.post1)
Requirement already satisfied: gast>=0.2.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (0.2.0)
Requirement already satisfied: absl-py>=0.1.6 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu) (0.1.12)
Requirement already satisfied: html5lib==0.9999999 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu) (0.9999999)
Requirement already satisfied: bleach==1.5.0 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu) (1.5.0)
Requirement already satisfied: werkzeug>=0.11.10 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu) (0.14.1)
Requirement already satisfied: markdown>=2.6.8 in /usr/local/lib/python3.6/dist-packages (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu) (2.6.11)
Requirement already satisfied: setuptools in /usr/local/lib/python3.6/dist-packages (from protobuf>=3.4.0->tensorflow-gpu) (39.0.1)
socketio 0.0.7 has requirement setuptools==3.3, but you'll have setuptools 39.0.1 which is incompatible.
root@DataLX01:~# 
~~~

root@DataLX01:~# apt-get install cuda-command-line-tools
~~~
패키지 목록을 읽는 중입니다... 완료
의존성 트리를 만드는 중입니다       
상태 정보를 읽는 중입니다... 완료
E: cuda-command-line-tools 패키지를 찾을 수 없습니다
~~~
root@DataLX01:~# apt-get install libcupti-dev
~~~
패키지 목록을 읽는 중입니다... 완료
의존성 트리를 만드는 중입니다       
상태 정보를 읽는 중입니다... 완료
다음 패키지가 자동으로 설치되었지만 더 이상 필요하지 않습니다:
  cuda-9-0 cuda-command-line-tools-9-0 cuda-core-9-0 cuda-cublas-9-0 cuda-cublas-dev-9-0 cuda-cudart-9-0
  cuda-cudart-dev-9-0 cuda-cufft-9-0 cuda-cufft-dev-9-0 cuda-curand-9-0 cuda-curand-dev-9-0 cuda-cusolver-9-0
  cuda-cusolver-dev-9-0 cuda-cusparse-9-0 cuda-cusparse-dev-9-0 cuda-demo-suite-9-0 cuda-documentation-9-0
  cuda-driver-dev-9-0 cuda-libraries-9-0 cuda-libraries-dev-9-0 cuda-license-9-0 cuda-misc-headers-9-0 cuda-npp-9-0
  cuda-npp-dev-9-0 cuda-nvgraph-9-0 cuda-nvgraph-dev-9-0 cuda-nvml-dev-9-0 cuda-nvrtc-9-0 cuda-nvrtc-dev-9-0
  cuda-runtime-9-0 cuda-samples-9-0 cuda-toolkit-9-0 cuda-visual-tools-9-0 libllvm4.0
Use 'apt autoremove' to remove them.
The following additional packages will be installed:
  libcupti-doc libcupti7.5
다음 새 패키지를 설치할 것입니다:
  libcupti-dev libcupti-doc libcupti7.5
0개 업그레이드, 3개 새로 설치, 0개 제거 및 48개 업그레이드 안 함.
1,113 k바이트 아카이브를 받아야 합니다.
이 작업 후 4,915 k바이트의 디스크 공간을 더 사용하게 됩니다.
계속 하시겠습니까? [Y/n] Y
받기:1 http://mirror.kakao.com/ubuntu xenial/multiverse amd64 libcupti7.5 amd64 7.5.18-0ubuntu1 [993 kB]
받기:2 http://mirror.kakao.com/ubuntu xenial/multiverse amd64 libcupti-dev amd64 7.5.18-0ubuntu1 [65.3 kB]
받기:3 http://mirror.kakao.com/ubuntu xenial/multiverse amd64 libcupti-doc all 7.5.18-0ubuntu1 [55.2 kB]
내려받기 1,113 k바이트, 소요시간 0초 (2,913 k바이트/초)
Selecting previously unselected package libcupti7.5:amd64.
(데이터베이스 읽는중 ...현재 356091개의 파일과 디렉터리가 설치되어 있습니다.)
Preparing to unpack .../libcupti7.5_7.5.18-0ubuntu1_amd64.deb ...
Unpacking libcupti7.5:amd64 (7.5.18-0ubuntu1) ...
Selecting previously unselected package libcupti-dev:amd64.
Preparing to unpack .../libcupti-dev_7.5.18-0ubuntu1_amd64.deb ...
Unpacking libcupti-dev:amd64 (7.5.18-0ubuntu1) ...
Selecting previously unselected package libcupti-doc.
Preparing to unpack .../libcupti-doc_7.5.18-0ubuntu1_all.deb ...
Unpacking libcupti-doc (7.5.18-0ubuntu1) ...
Processing triggers for libc-bin (2.23-0ubuntu10) ...
/sbin/ldconfig.real: file /usr/local/cuda-9.1/targets/x86_64-linux/lib/libcudnn.so.7 is truncated

libcupti7.5:amd64 (7.5.18-0ubuntu1) 설정하는 중입니다 ...
libcupti-dev:amd64 (7.5.18-0ubuntu1) 설정하는 중입니다 ...
libcupti-doc (7.5.18-0ubuntu1) 설정하는 중입니다 ...
Processing triggers for libc-bin (2.23-0ubuntu10) ...
/sbin/ldconfig.real: file /usr/local/cuda-9.1/targets/x86_64-linux/lib/libcudnn.so.7 is truncated

root@DataLX01:~# 
~~~

root@DataLX01:~# easy_install -U pip
~~~
Searching for pip
Reading https://pypi.python.org/simple/pip/
Downloading https://files.pythonhosted.org/packages/0f/74/ecd13431bcc456ed390b44c8a6e917c1820365cbebcb6a8974d1cd045ab4/pip-10.0.1-py2.py3-none-any.whl#sha256=717cdffb2833be8409433a93746744b59505f42146e8d37de6c62b430e25d6d7
Best match: pip 10.0.1
Processing pip-10.0.1-py2.py3-none-any.whl
Installing pip-10.0.1-py2.py3-none-any.whl to /usr/local/lib/python3.6/dist-packages
writing requirements to /usr/local/lib/python3.6/dist-packages/pip-10.0.1-py3.6.egg/EGG-INFO/requires.txt
Adding pip 10.0.1 to easy-install.pth file
Installing pip script to /usr/local/bin
Installing pip3 script to /usr/local/bin
Installing pip3.6 script to /usr/local/bin

Installed /usr/local/lib/python3.6/dist-packages/pip-10.0.1-py3.6.egg
Processing dependencies for pip
Finished processing dependencies for pip
root@DataLX01:~# 
~~~

root@DataLX01:~/installer# pip install tensorflow-gpu
~~~
Collecting tensorflow-gpu
  Downloading tensorflow_gpu-1.6.0-cp36-cp36m-manylinux1_x86_64.whl (209.2MB)
    100% |████████████████████████████████| 209.2MB 9.1kB/s
Collecting termcolor>=1.1.0 (from tensorflow-gpu)
  Downloading termcolor-1.1.0.tar.gz
Requirement already satisfied: six>=1.10.0 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu)
Collecting protobuf>=3.4.0 (from tensorflow-gpu)
  Downloading protobuf-3.5.2.post1-cp36-cp36m-manylinux1_x86_64.whl (6.4MB)
    100% |████████████████████████████████| 6.4MB 301kB/s
Collecting astor>=0.6.0 (from tensorflow-gpu)
  Downloading astor-0.6.2-py2.py3-none-any.whl
Requirement already satisfied: wheel>=0.26 in /usr/lib/python3/dist-packages (from tensorflow-gpu)
Collecting grpcio>=1.8.6 (from tensorflow-gpu)
  Downloading grpcio-1.10.0-cp36-cp36m-manylinux1_x86_64.whl (7.5MB)
    100% |████████████████████████████████| 7.5MB 260kB/s
Collecting absl-py>=0.1.6 (from tensorflow-gpu)
  Downloading absl-py-0.1.12.tar.gz (79kB)
    100% |████████████████████████████████| 81kB 8.5MB/s
Collecting tensorboard<1.7.0,>=1.6.0 (from tensorflow-gpu)
  Downloading tensorboard-1.6.0-py3-none-any.whl (3.0MB)
    100% |████████████████████████████████| 3.1MB 641kB/s
Collecting gast>=0.2.0 (from tensorflow-gpu)
  Downloading gast-0.2.0.tar.gz
Requirement already satisfied: numpy>=1.13.3 in /usr/local/lib/python3.6/dist-packages (from tensorflow-gpu)
Requirement already satisfied: setuptools in /usr/local/lib/python3.6/dist-packages (from protobuf>=3.4.0->tensorflow-gpu)
Collecting html5lib==0.9999999 (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu)
  Downloading html5lib-0.9999999.tar.gz (889kB)
    100% |████████████████████████████████| 890kB 1.8MB/s
Collecting bleach==1.5.0 (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu)
  Downloading bleach-1.5.0-py2.py3-none-any.whl
Collecting markdown>=2.6.8 (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu)
  Downloading Markdown-2.6.11-py2.py3-none-any.whl (78kB)
    100% |████████████████████████████████| 81kB 6.8MB/s
Collecting werkzeug>=0.11.10 (from tensorboard<1.7.0,>=1.6.0->tensorflow-gpu)
  Downloading Werkzeug-0.14.1-py2.py3-none-any.whl (322kB)
    100% |████████████████████████████████| 327kB 4.1MB/s
Building wheels for collected packages: termcolor, absl-py, gast, html5lib
  Running setup.py bdist_wheel for termcolor ... done
  Stored in directory: /root/.cache/pip/wheels/de/f7/bf/1bcac7bf30549e6a4957382e2ecab04c88e513117207067b03
  Running setup.py bdist_wheel for absl-py ... done
  Stored in directory: /root/.cache/pip/wheels/d6/d5/fc/8405dfaa90e82a8665116b5058e14891c37b4a0a707e03b634
  Running setup.py bdist_wheel for gast ... done
  Stored in directory: /root/.cache/pip/wheels/8e/fa/d6/77dd17d18ea23fd7b860e02623d27c1be451521af40dd4a13e
  Running setup.py bdist_wheel for html5lib ... done
  Stored in directory: /root/.cache/pip/wheels/6f/85/6c/56b8e1292c6214c4eb73b9dda50f53e8e977bf65989373c962
Successfully built termcolor absl-py gast html5lib
Installing collected packages: termcolor, protobuf, astor, grpcio, absl-py, html5lib, bleach, markdown, werkzeug, tensorboard, gast, tensorflow-gpu
  Found existing installation: html5lib 1.0.1
    Uninstalling html5lib-1.0.1:
      Successfully uninstalled html5lib-1.0.1
  Found existing installation: bleach 2.1.3
    Uninstalling bleach-2.1.3:
      Successfully uninstalled bleach-2.1.3
Successfully installed absl-py-0.1.12 astor-0.6.2 bleach-1.5.0 gast-0.2.0 grpcio-1.10.0 html5lib-0.9999999 markdown-2.6.11 protobuf-3.5.2.post1 tensorboard-1.6.0 tensorflow-gpu-1.6.0 termcolor-1.1.0 werkzeug-0.14.1
~~~
root@DataLX01:~/installer# apt list cuda*
~~~
Listing... 완료
cuda/unknown,now 9.1.85-1 amd64 [installed]
cuda-8-0/unknown 8.0.61-1 amd64
cuda-9-0/unknown,now 9.0.176-1 amd64 [installed,auto-removable]
cuda-9-1/unknown,now 9.1.85-1 amd64 [installed,automatic]
cuda-command-line-tools-8-0/unknown 8.0.61-1 amd64
cuda-command-line-tools-9-0/unknown,now 9.0.176-1 amd64 [installed,auto-removable]
cuda-command-line-tools-9-1/unknown,now 9.1.85-1 amd64 [installed,automatic]
~~~
