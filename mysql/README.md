#mysql

##Compiled from
<pre>community-mysql-5.7.17-1.fc26.src.rpm</pre>

##Modified
<pre>
- Package name
- %bcond_without config
- `mysql' requires `mysql-libs'
- `mysql-libs' requires `mysql-config'
- Disable test `main.grant_user_lock' (tries to log in as anonymous user, but is rerouted to root@localhost)
</pre>
