#openvas-manager

##Compiled from
<pre>openvas-manager-6.0.9-1.fc26.src.rpm</pre>

##Modified
<pre>
- Added openvas-manager.initd from Fedora git repository
- BuildRequires: sqlite-devel >= 3.7.15 (sqlite3_errstr() interface)
- Requires: sqlite >= 3.7.15 (sqlite-libs >= 3.11.0-3)
- Added '-fno-strict-aliasing' to avoid strict-aliasing errors
- Added a patch to fix a warn_unused_result error in src/manage_sql.c:2556
</pre>
