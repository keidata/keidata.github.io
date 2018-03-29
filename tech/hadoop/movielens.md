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
$ tail xaa
~~~
832|Bogus (1996)|06-Sep-1996||http://us.imdb.com/M/title-exact?Bogus%20(1996)|0|0|0|0|1|0|0|0|1|1|0|0|0|0|0|0|0|0|0
833|Bulletproof (1996)|06-Sep-1996||http://us.imdb.com/M/title-exact?Bulletproof%20(1996)|0|1|0|0|0|0|0|0|0|0|0|0|0|0|0|0|0|0|0
834|Halloween: The Curse of Michael Myers (1995)|01-Jan-1995||http://us.imdb.com/M/title-exact?Halloween:%20The%20Curse%20of%20Michael%20Myers%20(1995)|0|0|0|0|0|0|0|0|0|0|0|1|0|0|0|0|1|0|0
835|Gay Divorcee, The (1934)|01-Jan-1934||http://us.imdb.com/M/title-exact?Gay%20Divorcee%2C%20The%20%281934%29|0|0|0|0|0|1|0|0|0|0|0|0|1|0|1|0|0|0|0
836|Ninotchka (1939)|01-Jan-1939||http://us.imdb.com/M/title-exact?Ninotchka%20(1939)|0|0|0|0|0|1|0|0|0|0|0|0|0|0|1|0|0|0|0
837|Meet John Doe (1941)|01-Jan-1941||http://us.imdb.com/M/title-exact?Meet%20John%20Doe%20(1941)|0|0|0|0|0|0|0|0|1|0|0|0|0|0|0|0|0|0|0
838|In the Line of Duty 2 (1987)|30-Aug-1996||http://us.imdb.com/M/title-exact?In%20the%20Line%20of%20Duty%202%20(1987)|0|1|0|0|0|0|0|0|0|0|0|0|0|0|0|0|0|0|0
839|Loch Ness (1995)|01-Jan-1995||http://us.imdb.com/M/title-exact?Loch%20Ness%20(1995)|0|0|0|0|0|0|0|0|0|0|0|1|0|0|0|0|1|0|0
840|Last Man Standing (1996)|20-Sep-1996||http://us.imdb.com/M/title-exact?Last%20Man%20Standing%20(1996/I)|0|1|0|0|0|0|0|0|1|0|0|0|0|0|0|0|0|0|1
841|Glimmer Man, The (1996)|04-Oct-1996||http://us.imdb.com/M/title-exact?Glimmer%20Man,%20The%20(1996)|0|1|0|0|0|0|0|0|0|0|0|0|0|0|0|0|1|0|0
~~~
KODB@KDATA /cygdrive/c/Users/user/downloads/Hive/ml-100k
$ head xab
~~~
842|Pollyanna (1960)|01-Jan-1960||http://us.imdb.com/M/title-exact?Pollyanna%20(1960)|0|0|0|0|1|1|0|0|1|0|0|0|0|0|0|0|0|0|0
843|Shaggy Dog, The (1959)|01-Jan-1959||http://us.imdb.com/M/title-exact?Shaggy%20Dog,%20The%20(1959)|0|0|0|0|1|1|0|0|0|0|0|0|0|0|0|0|0|0|0
844|Freeway (1996)|23-Aug-1996||http://us.imdb.com/M/title-exact?Freeway%20(1996)|0|0|0|0|0|0|1|0|0|0|0|0|0|0|0|0|0|0|0
845|That Thing You Do! (1996)|28-Sep-1996||http://us.imdb.com/M/title-exact?That%20Thing%20You%20Do!%20(1996)|0|0|0|0|0|1|0|0|0|0|0|0|0|0|0|0|0|0|0
846|To Gillian on Her 37th Birthday (1996)|18-Oct-1996||http://us.imdb.com/M/title-exact?To%20Gillian%20on%20Her%2037th%20Birthday%20(1996)|0|0|0|0|0|0|0|0|1|0|0|0|0|0|1|0|0|0|0
847|Looking for Richard (1996)|11-Oct-1996||http://us.imdb.com/M/title-exact?Looking%20for%20Richard%20(1996)|0|0|0|0|0|0|0|1|1|0|0|0|0|0|0|0|0|0|0
848|Murder, My Sweet (1944)|01-Jan-1944||http://us.imdb.com/M/title-exact?Murder,%20My%20Sweet%20(1944)|0|0|0|0|0|0|0|0|0|0|1|0|0|0|0|0|1|0|0
849|Days of Thunder (1990)|01-Jan-1990||http://us.imdb.com/M/title-exact?Days%20of%20Thunder%20(1990)|0|1|0|0|0|0|0|0|0|0|0|0|0|0|1|0|0|0|0
850|Perfect Candidate, A (1996)|27-Sep-1996||http://us.imdb.com/M/title-exact?Perfect%20Candidate,%20A%20(1996)|0|0|0|0|0|0|0|1|0|0|0|0|0|0|0|0|0|0|0
851|Two or Three Things I Know About Her (1966)|01-Jan-1966||http://us.imdb.com/M/title-exact?Deux%20ou%20trois%20choses%20que%20je%20sais%20d'elle%20(1966)|0|0|0|0|0|0|0|0|1|0|0|0|0|0|0|0|0|0|0
~~~
KODB@KDATA /cygdrive/c/Users/user/downloads/Hive/ml-100k
$
