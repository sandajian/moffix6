#gcc

##Compiled from
<pre>gcc-6.3.1-1.fc26.src.rpm</pre>

##Modified
<pre>
- %global build_libstdcxx_docs 0
- BuildRequires: hostname -> /bin/hostname
- BuildRequires: python3-devel -> python34-devel
- Remove: Requires: filesystem >= 3
- /usr/lib/cpp -> /lib/cpp: 'rpcgen' cannot find any C preprocessor (cpp)
</pre>

##Notes
<pre>
- BuildRequires: libmpc-devel >= 0.8.1, the latest compatible version is:
	libmpc-0.9-3.fc18.2.src.rpm, which requires gmp-devel >= 4.3.2, mpfr-devel >= 2.4.2
- When you try to install(update) these rpms after building for the first time, 'gettext' and 'libtool' would get broken dependencies.  You may just add '--nodeps' to force installation first, then recompile 'gettext' and 'libtool' using the new version of gcc.
</pre>
