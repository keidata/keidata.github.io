root@DataLX01:~# pip list | grep ros
~~~
rospkg                        1.1.4                 
~~~
root@DataLX01:~# pip install rosdep
~~~
Looking in indexes: http://ftp.daumkakao.com/pypi/simple
Collecting rosdep
  Downloading http://mirror.kakao.com/pypi/packages/02/b7/c54f4cfed18f3367be992f74298c2ceb60a679c7e5982f2ba79fbd289ee9/rosdep-0.12.2.tar.gz (80kB)
    100% |████████████████████████████████| 81kB 1.4MB/s 
Collecting catkin_pkg (from rosdep)
  Downloading http://mirror.kakao.com/pypi/packages/13/c0/429e0517247c820912e23cab56f733433372828a135303a63c0fd319bed3/catkin_pkg-0.4.1.tar.gz (49kB)
    100% |████████████████████████████████| 51kB 4.2MB/s 
Requirement already satisfied: rospkg>=1.0.37 in /usr/local/lib/python3.6/dist-packages (from rosdep) (1.1.4)
Collecting rosdistro>=0.4.0 (from rosdep)
  Downloading http://mirror.kakao.com/pypi/packages/15/3f/6053492e43fb6b9625f57fc72772f333e58a4ff08f96d400361491fce486/rosdistro-0.6.8.tar.gz (44kB)
    100% |████████████████████████████████| 51kB 17.0MB/s 
Requirement already satisfied: PyYAML>=3.1 in /usr/local/lib/python3.6/dist-packages (from rosdep) (3.12)
Requirement already satisfied: argparse in /usr/local/lib/python3.6/dist-packages (from catkin_pkg->rosdep) (1.4.0)
Requirement already satisfied: docutils in /usr/local/lib/python3.6/dist-packages (from catkin_pkg->rosdep) (0.14)
Requirement already satisfied: python-dateutil in /usr/local/lib/python3.6/dist-packages (from catkin_pkg->rosdep) (2.7.0)
Requirement already satisfied: pyparsing in /usr/lib/python3/dist-packages (from catkin_pkg->rosdep) (2.0.3)
Requirement already satisfied: setuptools in /usr/local/lib/python3.6/dist-packages (from rosdistro>=0.4.0->rosdep) (39.0.1)
Requirement already satisfied: six>=1.5 in /usr/local/lib/python3.6/dist-packages (from python-dateutil->catkin_pkg->rosdep) (1.11.0)
Building wheels for collected packages: rosdep, catkin-pkg, rosdistro
  Running setup.py bdist_wheel for rosdep ... done
  Stored in directory: /root/.cache/pip/wheels/f3/95/84/e4d0a845255a97e5b210a0487ffe1e15493d2b97df5836ca50
  Running setup.py bdist_wheel for catkin-pkg ... done
  Stored in directory: /root/.cache/pip/wheels/b8/8e/ea/dc7486959e0dafd5a06fb7e62315630ebce35e956510b98feb
  Running setup.py bdist_wheel for rosdistro ... done
  Stored in directory: /root/.cache/pip/wheels/03/10/58/cadab6ba8dbe67e101a8b24c4bdcc368b01336bed4305205ce
Successfully built rosdep catkin-pkg rosdistro
socketio 0.0.7 has requirement setuptools==3.3, but you'll have setuptools 39.0.1 which is incompatible.
Installing collected packages: catkin-pkg, rosdistro, rosdep
Successfully installed catkin-pkg-0.4.1 rosdep-0.12.2 rosdistro-0.6.8
~~~
root@DataLX01:~# pip install rosdistro
~~~
Looking in indexes: http://ftp.daumkakao.com/pypi/simple
Requirement already satisfied: rosdistro in /usr/local/lib/python3.6/dist-packages (0.6.8)
Requirement already satisfied: setuptools in /usr/local/lib/python3.6/dist-packages (from rosdistro) (39.0.1)
Requirement already satisfied: catkin-pkg in /usr/local/lib/python3.6/dist-packages (from rosdistro) (0.4.1)
Requirement already satisfied: PyYAML in /usr/local/lib/python3.6/dist-packages (from rosdistro) (3.12)
Requirement already satisfied: rospkg in /usr/local/lib/python3.6/dist-packages (from rosdistro) (1.1.4)
Requirement already satisfied: docutils in /usr/local/lib/python3.6/dist-packages (from catkin-pkg->rosdistro) (0.14)
Requirement already satisfied: pyparsing in /usr/lib/python3/dist-packages (from catkin-pkg->rosdistro) (2.0.3)
Requirement already satisfied: python-dateutil in /usr/local/lib/python3.6/dist-packages (from catkin-pkg->rosdistro) (2.7.0)
Requirement already satisfied: argparse in /usr/local/lib/python3.6/dist-packages (from catkin-pkg->rosdistro) (1.4.0)
Requirement already satisfied: six>=1.5 in /usr/local/lib/python3.6/dist-packages (from python-dateutil->catkin-pkg->rosdistro) (1.11.0)
socketio 0.0.7 has requirement setuptools==3.3, but you'll have setuptools 39.0.1 which is incompatible.
~~~
root@DataLX01:~# pip list | grep ros
~~~
rosdep                        0.12.2                
rosdistro                     0.6.8                 
rospkg                        1.1.4                 
~~~
