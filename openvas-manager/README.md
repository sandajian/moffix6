#openvas-manager

##Compiled from
<pre>openvas-manager-6.0.9-1.fc26.src.rpm</pre>

##Modified
<pre>
- Added openvas-manager.initd from Fedora git repository
- BuildRequires: sqlite-devel >= 3.7.15 (sqlite3_errstr() interface)
- Requires: sqlite >= 3.7.15 (sqlite-libs >= 3.11.0-3)
- Added '-Wno-error=unused-result': src/manage_sql.c:2656: strtol (stripped, &stripped_end, 10);
- Add a patch to avoid strict-aliasing errors when compiled with GCC 4.4.7. Remove '-Werror=unused-but-set-variable'
</pre>

##Notes
<pre>
- !!! Use 'rpmbuild -ba ...' to include openvas-manager.initd in .src.rpm
</pre>
