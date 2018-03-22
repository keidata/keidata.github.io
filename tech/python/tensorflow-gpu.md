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
