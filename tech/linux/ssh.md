### SSH 사용 시 Key로 인증하기 
- https://arsviator.blogspot.kr/2015/04/ssh-ssh-key.html  
  
[vagrant@nn01 .ssh]$ ssh-keygen
~~~
Generating public/private rsa key pair.
Enter file in which to save the key (/home/vagrant/.ssh/id_rsa): 
/home/vagrant/.ssh/id_rsa already exists.
Overwrite (y/n)? y
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/vagrant/.ssh/id_rsa.
Your public key has been saved in /home/vagrant/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:yaq9RdexFXGELhQjUyeFAkGjKb/r2A3B3xSfw7KHa6U vagrant@nn01
The key's randomart image is:
+---[RSA 2048]----+
|       .=oo.=+=+o|
|       o ..oo+.o |
|    . o   .o...  |
|     + . . =.=.  |
|      + S + B.   |
|       * + +..   |
|      + o +o.    |
|     = =  Eo     |
|    o.*....      |
+----[SHA256]-----+
~~~
[vagrant@nn01 .ssh]$ sudo scp ~/.ssh/id_rsa.pub vagrant@dn01:/tmp/id_rsa_nn01.pub
~~~
vagrant@dn01's password: 
id_rsa.pub                                           100%  394   595.5KB/s   00:00    
~~~
[vagrant@nn01 .ssh]$ sudo scp ~/.ssh/id_rsa.pub vagrant@dn02:/tmp/id_rsa_nn01.pub
~~~
vagrant@dn02's password: 
id_rsa.pub                                           100%  394   657.9KB/s   00:00  
~~~
[vagrant@dn01 ~]$ cat /tmp/id_rsa_nn01.pub >> ~/.ssh/authorized_keys  
  
[vagrant@dn02 ~]$ cat /tmp/id_rsa_nn01.pub >> ~/.ssh/authorized_keys  
