#ocaml

##Compiled from
<pre>ocaml-4.02.3-3.fc25.src.rpm</pre>

##Modified
<pre>
- BuildRequires:  ocaml-srpm-macros
</pre>

##Notes
<pre>
- Do not use --rebuild, unpack src.rpm and use rpmbuild -ba. Or else `Provides:' will not be generated correctly.
- ocaml-4.04.0-7.fc26.src.rpm causes an error when compiling hhvm:
	heap/hh_shared.c: In function ‘raise_less_than_minimum_available’:
	heap/hh_shared.c:489: error: ‘caml__frame’ undeclared (first use in this function)
</pre>
