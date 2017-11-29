<code><b>[root@stdalonejq krb5kdc]# kinit jcquevedo</b></code><br>
Password for jcquevedo@RAKENHDP.COM: <br>
<br>
<code><b>[root@stdalonejq krb5kdc]# klist -fe</b></code><br>
Ticket cache: KEYRING:persistent:0:0<br>
Default principal: jcquevedo@RAKENHDP.COM<br>

Valid starting     Expires            Service principal<br>
11/29/17 16:40:43  11/30/17 16:40:43  krbtgt/RAKENHDP.COM@RAKENHDP.COM<br>
	renew until 12/06/17 16:40:43, Flags: FRI<br>
	Etype (skey, tkt): arcfour-hmac, aes256-cts-hmac-sha1-96 <br>
[root@stdalonejq krb5kdc]# <br>
<br>

<code><b>kadmin.local:  getprinc jcquevedo</b></code><br>
Principal: jcquevedo@RAKENHDP.COM<br>
Expiration date: [never]<br>
Last password change: Wed Nov 29 15:57:17 EST 2017<br>
Password expiration date: [never]<br>
Maximum ticket life: 1 day 00:00:00<br>
Maximum renewable life: 7 days 00:00:00<br>
Last modified: Wed Nov 29 15:57:18 EST 2017 (root/admin@RAKENHDP.COM)<br>
Last successful authentication: [never]<br>
Last failed authentication: [never]<br>
Failed password attempts: 0<br>
Number of keys: 8<br>
Key: vno 1, aes256-cts-hmac-sha1-96<br>
Key: vno 1, aes128-cts-hmac-sha1-96<br>
Key: vno 1, des3-cbc-sha1<br>
Key: vno 1, arcfour-hmac<br>
Key: vno 1, camellia256-cts-cmac<br>
Key: vno 1, camellia128-cts-cmac<br>
Key: vno 1, des-hmac-sha1<br>
Key: vno 1, des-cbc-md5<br>
MKey: vno 1<br>
Attributes:<br>
Policy: [none]<br>
kadmin.local:  <br>


