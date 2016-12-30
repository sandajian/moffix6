#mariadb

##Compiled from
<pre>mariadb-10.1.20-1.fc26.src.rpm</pre>

##Modified
<pre>
- Without `tokudb', for g++ 4.4.7 does not support designated initializers.
- Remove test `plugins.feedback_plugin_load'
	plugins.feedback_plugin_load test failed:
		Warning        1265    Data truncated for column 'VARIABLE_VALUE' at row 498
- Remove systemd-releated files
- 'mariadb' requires 'mariadb-config' and 'mariadb-libs'
- 'mariadb-libs' requires 'mariadb-config'
- Fix a '%{_pkgdocdir}' related issue.
</pre>

##Notes
<pre>
- Designated initializers:
	struct a {int b; int c; };
	struct a d = { .b=1, .c=2 };
	int main() { return 0; }
</pre>
