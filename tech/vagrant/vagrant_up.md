C:\Users\user\vagrant>tree
~~~
폴더 PATH의 목록입니다.
볼륨 일련 번호는 4074-D233입니다.
C:.
├─hadoop
│  ├─.vagrant
│  │  └─machines
│  │      └─default
│  │          └─virtualbox
│  ├─resources
│  │  ├─hadoop
│  │  │  ├─config
│  │  │  └─install
│  │  └─jdk
│  └─scripts
└─jdk
~~~
C:\Users\user\vagrant>cd hadoop
  
C:\Users\user\vagrant\hadoop>vagrant box list
~~~
centos7 (virtualbox, 0)
~~~
C:\Users\user\vagrant\hadoop>vagrant up dn01 dn02 nn01 > hive.log
  
C:\Users\user\vagrant\hadoop>
