#mariadb

##Compiled from
<pre><code>mariadb-10.1.19-3.fc26.src.rpm</code></pre>

##Modified

<pre>
	BuildRequires: openssl, openssl-devel
	Without `tokudb'
	Remove test `plugins.feedback_plugin_load'
		plugins.feedback_plugin_load test failed:
			Warning        1265    Data truncated for column 'VARIABLE_VALUE' at row 498
	Remove systemd-releated files
</pre>
