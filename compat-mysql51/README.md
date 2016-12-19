#compat-mysql51

##Compiled from
<pre>compat-mysql51-5.1.54-1.remi.src.rpm</pre>

##Notes
<pre>
- When building with gcc-6.2.1, use rpmbuild --define='optflags -Wno-narrowing' to avoid errors:

mysqlbinlog.cc:1148:1: error: narrowing conversion of '18446744073709551615ull' from 'ulonglong {aka long long unsigned int}' to 'longlong {aka long long int}' inside { } [-Wnarrowing]
mysql.cc:1565:1: error: narrowing conversion of '18446744073709551615ul' from 'long unsigned int' to 'longlong {aka long long int}' inside { } [-Wnarrowing]

</pre>
