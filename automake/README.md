#automake

##Compiled from
<pre>automake-1.15-8.fc26.src.rpm</pre>

##Modified
<pre>
- Remove 'BuildRequires: perl-macros'
- Add a blank line after '%autosetup -p1'
- Do not 'autoreconf -iv', use './bootstrap.sh' instead.
</pre>

##Notes
<pre>
- 'autoreconf -iv' produces: automake: cannot open < ./%D%/automake.texi: No such file or directory
- If automake is updated, we may recompile automake with 'autoreconf -iv'
</pre>
