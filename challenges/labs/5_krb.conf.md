<code><b>[root@host1 CDH5]# vi /etc/krb5.conf</b></code><br>

[libdefaults]<br>
default_realm = JCQUEVEDO.HQ.COM<br>
dns_lookup_kdc = false<br>
dns_lookup_realm = false<br>
ticket_lifetime = 86400<br>
renew_lifetime = 604800<br>
forwardable = true<br>
default_tgs_enctypes = arcfour-hmac<br>
default_tkt_enctypes = arcfour-hmac<br>
permitted_enctypes = arcfour-hmac<br>
udp_preference_limit = 1<br>
kdc_timeout = 3000<br>
[realms]<br>
JCQUEVEDO.HQ.COM = {<br>
kdc = stdalonejq.northcentralus.cloudapp.azure.com<br>
admin_server = stdalonejq.northcentralus.cloudapp.azure.com<br>
}<br>
