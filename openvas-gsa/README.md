#openvas-gsa

##Compiled from
<pre>openvas-gsa-6.0.11-3.fc26.src.rpm</pre>

##Modified
<pre>
- Added openvas-gsa.initd from Fedora git repository
- Removed Requires: texlive-changepage, texlive-comment, added Requires: texlive-texmf-latex
- Patched src/gsad.c to avoid strict-aliasing errors when compiled with GCC 4.4.7
</pre>

##Notes
<pre>
- !!! Use 'rpmbuild -ba ...' to include openvas-gsa.initd in .src.rpm
</pre>
