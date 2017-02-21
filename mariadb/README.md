#mariadb

##Compiled from
<pre>mariadb-10.1.21-3.fc25.src.rpm</pre>

##Modified
<pre>
- Remove test `plugins.feedback_plugin_load'
	plugins.feedback_plugin_load test failed:
		Warning        1265    Data truncated for column 'VARIABLE_VALUE' at row 498
- Remove systemd-releated files
- 'mariadb' requires 'mariadb-config'
- 'mariadb-libs' requires 'mariadb-config'
</pre>

##Notes
<pre>
- Using gcc 6.3.1
- g++ 4.4.7 does not support designated initializers, so 'without tokudb'
- Designated initializers:
	struct a {int b; int c; };
	struct a d = { .b=1, .c=2 };
	int main() { return 0; }
</pre>
