<code><b>[root@stdalonejq krb5kdc]# cat kdc.conf </b></code><br>
[kdcdefaults]<br>
 kdc_ports = 88<br>
 kdc_tcp_ports = 88<br>

[realms]<br>
 JCQUEVEDO.HQ.COM = {<br>
  #master_key_type = aes256-cts<br>
  acl_file = /var/kerberos/krb5kdc/kadm5.acl<br>
  dict_file = /usr/share/dict/words<br>
  admin_keytab = /var/kerberos/krb5kdc/kadm5.keytab<br>
  supported_enctypes = aes256-cts:normal aes128-cts:normal des3-hmac-sha1:normal arcfour-hmac:normal camellia256-cts:normal<br> camellia128-cts:normal des-hmac-sha1:normal des-cbc-md5:normal des-cbc-crc:normal<br>
  max_life = 1d<br>
  max_renewable_life = 7d<br>
 }<br>
[root@stdalonejq krb5kdc]# <br>
