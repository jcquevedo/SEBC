<b> Final run with 0.9 multiplier </b><br>
<code><b>[raken@hdp1 ~]$ HADOOP_USER_NAME=jcquevedo ./3_YARNtest.sh </b></code><br>
Testing loop started on Tue Nov 28 16:41:16 EST 2017<br>
Memory=  512<br>
Job Tasks= 8<br>
Map Memory= 460<br>
Reduce Memory= 460<br>

real	1m2.935s<br>
user	0m5.225s<br>
sys	0m0.299s<br>

real	2m31.947s<br>
user	0m7.631s<br>
sys	0m0.435s<br>
Deleted /user/jcquevedo/results/tg-10GB-8-1-512<br>
Deleted /user/jcquevedo/results/ts-10GB-8-1-512<br>
Memory=  1024<br>
Job Tasks= 8<br>
Map Memory= 921<br>
Reduce Memory= 921<br>

real	1m6.354s<br>
user	0m5.185s<br>
sys	0m0.318s<br>

real	2m44.287s<br>
user	0m7.646s<br>
sys	0m0.390s<br>
Deleted /user/jcquevedo/results/tg-10GB-8-1-1024<br>
Deleted /user/jcquevedo/results/ts-10GB-8-1-1024<br>
Testing loop ended on Tue Nov 28 16:48:50 EST 2017<br>


<b># We fixed Eco, now first run with proper Echo</b><br>
<code>[raken@hdp1 ~]$ HADOOP_USER_NAME=jcquevedo ./3_YARNtest.sh </code><br>
Testing loop started on Tue Nov 28 16:33:16 EST 2017<br>
Memory=  512<br>
Job Tasks= 8<br>
Map Memory= 409<br>
Reduce Memory= 409<br>

real	1m3.337s<br>
user	0m5.342s<br>
sys	0m0.321s<br>

real	2m14.874s<br>
user	0m7.329s<br>
sys	0m0.396s<br>
Deleted /user/jcquevedo/results/tg-10GB-8-1-512<br>
Deleted /user/jcquevedo/results/ts-10GB-8-1-512<br>
Memory=  1024<br>
Job Tasks= 8<br>
Map Memory= 819<br>
Reduce Memory= 819<br>

real	1m5.961s<br>
user	0m5.237s<br>
sys	0m0.323s<br>

real	2m32.885s<br>
user	0m7.743s<br>
sys	0m0.422s<br>
Deleted /user/jcquevedo/results/tg-10GB-8-1-1024<br>
Deleted /user/jcquevedo/results/ts-10GB-8-1-1024<br>
Testing loop ended on Tue Nov 28 16:40:22 EST 2017<br>



<b># At the time we first ran, we had a couple mistakes on echo </b><br>
<code><b>[raken@hdp1 ~]$ HADOOP_USER_NAME=jcquevedo ./3_YARNtest.sh </b></code><br>
Testing loop started on Tue Nov 28 16:10:25 EST 2017<br>
Job Tasks=  512<br>
Memory= 8<br>
Map Memory= 409<br>
Reduce Memory= 409<br>

real	1m6.950s<br>
user	0m4.864s<br>
sys	0m0.309s<br>

real	2m38.868s<br>
user	0m7.443s<br>
sys	0m0.431s<br>
Deleted /user/jcquevedo/results/tg-10GB-8-1-512<br>
Deleted /user/jcquevedo/results/ts-10GB-8-1-512<br>
Job Tasks=  1024<br>
Memory= 8<br>
Map Memory= 819<br>
Reduce Memory= 819<br>

real	1m8.017s<br>
user	0m5.051s<br>
sys	0m0.282s<br>

real	2m16.917s<br>
user	0m7.686s<br>
sys	0m0.403s<br>
Deleted /user/jcquevedo/results/tg-10GB-8-1-1024<br>
Deleted /user/jcquevedo/results/ts-10GB-8-1-1024<br>
Testing loop ended on Tue Nov 28 16:17:45 EST 2017<br>

<code><b>




