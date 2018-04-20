## Python 여러 버전 설치하기  
  
* 참고 : http://kalten.tistory.com/234
  
1) 버전 확인하기  
~~~
root@DataLX01:~# python -V
Python 2.7.12
root@DataLX01:~# python3 -V
Python 3.6.3
~~~
2) 여러 버전 지정하기
~~~
root@DataLX01:~# update-alternatives --config python
update-alternatives: 오류: no alternatives for python
root@DataLX01:~# update-alternatives --install /usr/bin/python python /usr/bin/python2.7 1
update-alternatives: using /usr/bin/python2.7 to provide /usr/bin/python (python) in auto mode
root@DataLX01:~# update-alternatives --install /usr/bin/python python /usr/bin/python3.5 2
update-alternatives: using /usr/bin/python3.5 to provide /usr/bin/python (python) in auto mode
root@DataLX01:~# update-alternatives --install /usr/bin/python python /usr/bin/python3.6 3
update-alternatives: using /usr/bin/python3.6 to provide /usr/bin/python (python) in auto mode
root@DataLX01:~# update-alternatives --config python
대체 항목 python에 대해 (/usr/bin/python 제공) 3개 선택이 있습니다.

  선택       경로              우선순

                                      ------------------------------------------------------------
* 0            /usr/bin/python3.6   3         자동 모드
  1            /usr/bin/python2.7   1         수동 모드
  2            /usr/bin/python3.5   2         수동 모드
  3            /usr/bin/python3.6   3         수동 모드

Press <enter> to keep the current choice[*], or type selection number: 
root@DataLX01:~#
~~~
