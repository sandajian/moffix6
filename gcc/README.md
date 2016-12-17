#gcc

##Compiled from
<pre>gcc-4.9.2-6.fc21.src.rpm</pre>

##Modified
<pre>
- %global build_libstdcxx_docs 0
- BuildRequires: /bin/hostname
- Remove: Requires: filesystem >= 3
</pre>

##Notes
<pre>
- When you try to install(update) these rpms after building, `gettext' and `libtool' would get broken dependencies.  You may just add `--nodeps' to force installation first, then recompile `gettext' and `libtool' using gcc-4.9.2.
</pre>
