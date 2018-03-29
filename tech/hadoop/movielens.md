KODB@KDATA /cygdrive/c/Users/user/downloads/Hive/ml-100k
$ wc -l u.user
~~~
943 u.user
~~~
KODB@KDATA /cygdrive/c/Users/user/downloads/Hive/ml-100k
$ head u.user
~~~
1|24|M|technician|85711
2|53|F|other|94043
3|23|M|writer|32067
4|24|M|technician|43537
5|33|F|other|15213
6|42|M|executive|98101
7|57|M|administrator|91344
8|36|M|administrator|05201
9|29|M|student|01002
10|53|M|lawyer|90703
~~~
KODB@KDATA /cygdrive/c/Users/user/downloads/Hive/ml-100k
$ wc -l u.item
~~~
1682 u.item
~~~
KODB@KDATA /cygdrive/c/Users/user/downloads/Hive/ml-100k
$ head u.item
~~~
1|Toy Story (1995)|01-Jan-1995||http://us.imdb.com/M/title-exact?Toy%20Story%20(1995)|0|0|0|1|1|1|0|0|0|0|0|0|0|0|0|0|0|0|0
2|GoldenEye (1995)|01-Jan-1995||http://us.imdb.com/M/title-exact?GoldenEye%20(1995)|0|1|1|0|0|0|0|0|0|0|0|0|0|0|0|0|1|0|0
3|Four Rooms (1995)|01-Jan-1995||http://us.imdb.com/M/title-exact?Four%20Rooms%20(1995)|0|0|0|0|0|0|0|0|0|0|0|0|0|0|0|0|1|0|0
4|Get Shorty (1995)|01-Jan-1995||http://us.imdb.com/M/title-exact?Get%20Shorty%20(1995)|0|1|0|0|0|1|0|0|1|0|0|0|0|0|0|0|0|0|0
5|Copycat (1995)|01-Jan-1995||http://us.imdb.com/M/title-exact?Copycat%20(1995)|0|0|0|0|0|0|1|0|1|0|0|0|0|0|0|0|1|0|0
6|Shanghai Triad (Yao a yao yao dao waipo qiao) (1995)|01-Jan-1995||http://us.imdb.com/Title?Yao+a+yao+yao+dao+waipo+qiao+(1995)|0|0|0|0|0|0|0|0|1|0|0|0|0|0|0|0|0|0|0
7|Twelve Monkeys (1995)|01-Jan-1995||http://us.imdb.com/M/title-exact?Twelve%20Monkeys%20(1995)|0|0|0|0|0|0|0|0|1|0|0|0|0|0|0|1|0|0|0
8|Babe (1995)|01-Jan-1995||http://us.imdb.com/M/title-exact?Babe%20(1995)|0|0|0|0|1|1|0|0|1|0|0|0|0|0|0|0|0|0|0
9|Dead Man Walking (1995)|01-Jan-1995||http://us.imdb.com/M/title-exact?Dead%20Man%20Walking%20(1995)|0|0|0|0|0|0|0|0|1|0|0|0|0|0|0|0|0|0|0
10|Richard III (1995)|22-Jan-1996||http://us.imdb.com/M/title-exact?Richard%20III%20(1995)|0|0|0|0|0|0|0|0|1|0|0|0|0|0|0|0|0|1|0
~~~
KODB@KDATA /cygdrive/c/Users/user/downloads/Hive/ml-100k
$ split.exe -l 841 u.item
  
KODB@KDATA /cygdrive/c/Users/user/downloads/Hive/ml-100k
$ ls
~~~
allbut.pl  u.data   u.item        u1.base  u2.test  u4.base  u5.test  ub.base  xab
mku.sh     u.genre  u.occupation  u1.test  u3.base  u4.test  ua.base  ub.test
README     u.info   u.user        u2.base  u3.test  u5.base  ua.test  xaa
~~~
KODB@KDATA /cygdrive/c/Users/user/downloads/Hive/ml-100k
$
