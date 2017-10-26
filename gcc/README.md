# gcc

## Compiled from
<pre>Fedora .src.rpm</pre>

## Modified
<pre>
- %global build_libstdcxx_docs 0
- BuildRequires: python3-devel -> python34-devel
- BuildRequires: hostname -> /bin/hostname
- Removed: Requires: filesystem >= 3
- Removed: Provides: /lib/cpp
- /usr/lib/cpp -> /lib/cpp: 'rpcgen' cannot find any C preprocessor (cpp)
</pre>

## Notes
<pre>
- BuildRequires: libmpc-devel >= 0.8.1, the latest compatible version is:
	libmpc-0.9-3.fc18.2.src.rpm, which requires gmp-devel >= 4.3.2, mpfr-devel >= 2.4.2
</pre>
