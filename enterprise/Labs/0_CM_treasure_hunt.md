<code><b>What is ubertask optimization?</b></code><br>
Jobs which meet "small" configuration defined by mapreduce.job.ubertask.maxmaps, mapreduce.job.ubertask.maxreduces, and mapreduce.job.ubertask.maxbytes settings runs sequentially in a single JVM.

<code><b>Where in CM is the Kerberos Security Realm value displayed?</b></code><br>
Administration -> Settings -> Scope Kerberos -> default_realm

<code><b>Which CDH service(s) host a property for enabling Kerberos authentication?</b></code><br>
All Services.

<code><b>How do you upgrade the CM agents?</b></code><br>
It can be done with the wizzard from CM Admin or Manually.

<code><b>Give the tsquery statement used to chart Hue's CPU utilization?</b></code><br>
select cpu_system_rate + cpu_user_rate where category=ROLE and serviceName=$SERVICENAME

<code><b>Name all the roles that make up the Hive service</b></code><br>
Hive Metastore Server, Hive Server2

<code><b>What steps must be completed before integrating Cloudera Manager with Kerberos?</b></code><br>
1.- Set up Working KDC <br>
2.- Check that KDC Allows Renewable Tickets<br>
3.- Install KDC Client Libraries on all hosts, Or LDAP Libraries on CM Server if using Active Directory<br>
4.-  Create an account for CM with create users privileges<br>
