#cmake

##Compiled from
<pre>cmake-3.7.0-1.fc26.src.rpm</pre>

##Modified
<pre>
- with bootstrap (do not use system-libs to avoid updating libuv)
</pre>

##Modified (use system-libs)
<pre>
- Added cmake-libarchive3.patch
- BuildRequires:  libuv-devel >= 1:1.0.0
</pre>

##Notes
<pre>
- DO NOT USE root to compile
</pre>
