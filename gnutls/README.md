#gnutls

##Compiled from
<pre>gnutls-2.12.23-2.fc18.src.rpm</pre>

##Modified
<pre>
- Requires: libtasn1 >= 2.14
</pre>

##Requires
<pre>
- libtasn1-devel >= 2.14
</pre>

##Notes
<pre>
- gnutls-2.12.23-2 is the latest compatible version that provides libgnutls.so.26
- Removed: export LDFLAGS="-Wl,--no-add-needed", when using system-default binutils:

When using system-default binutils-2.20.51.0.2, with LDFLAGS="-Wl,--no-add-needed", there is a linker error:

  CXXLD  ex-cxx
/usr/bin/ld: ex-cxx: undefined reference to symbol 'pthread_cancel@@GLIBC_2.2.5'
/usr/bin/ld: note: 'pthread_cancel@@GLIBC_2.2.5' is defined in DSO /lib64/libpthread.so.0 so try adding it to the linker command line
/lib64/libpthread.so.0: could not read symbols: Invalid operation

When using binutils-2.27, link OK.
</pre>
