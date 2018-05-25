## slam과 tm이 설치가 잘 안 된다.
  
1) r-base 업그레이드 하라는데, 별로 도움은 안 되는 것 같고  
~~~
root@DataLX01:~# apt show r-base
Package: r-base
Version: 3.4.3-1xenial0
Status: install ok installed
.......
~~~
2) 


~~~
root@DataLX01:~# ldconfig -p | grep libgfortran
        libgfortran.so.3 (libc6,x32) => /usr/libx32/libgfortran.so.3
        libgfortran.so.3 (libc6,x86-64) => /usr/lib/x86_64-linux-gnu/libgfortran.so.3
        libgfortran.so.3 (libc6) => /usr/lib32/libgfortran.so.3
~~~
