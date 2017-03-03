#pam_mysql

##Compiled from
<pre>pam_mysql-0.7-0.21.rc1.fc24.src.rpm</pre>

##Modified
<pre>
- Added '-lpam' to avoid the following error:
		/lib64/security/pam_mysql.so: undefined symbol: pam_set_data
</pre>
