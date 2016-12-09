#Moffix6 - a repository that provides updated packages of CentOS 6 x86_64

(NOTE: packages uploading in progress, please wait for a day or two ...)


Although CentOS 7 has released for years, I'm still sticking on CentOS 6.  The reasons may be:

1. Our business are running on CentOS 6, upgrading would be costing.
2. I hate systemd, or some other features of CentOS 7.
3. Whatever, I like CentOS 6.

OK, I decide to use CentOS 6 for a little more time.  But CentOS 6 is too old, many libraries and software are outdated.  New software need new versions of libraries and tools.  Some RPMs can be downloaded after searching the internet, others need to be compiled by myself.

This repository originally comes from the compilation of Facebook HHVM on CentOS 6.  To solve the dependencies, I need to compile a lot of packages from SRPMs, with modifications of some spec files or source codes.

In order to use this repository, your system should meet:

1. CentOS 6.x x86_64
2. Epel 6 x86_64

Download repo file from:

	https://copr.fedorainfracloud.org/coprs/chenxy/moffix6/repo/epel-6/chenxy-moffix6-epel-6.repo

If you want to recompile packages, you should following a special sequence of building:

1. install `epel-rpm-macros' to resolve rpm macros like '%make_build' and '%license'.
2. Rebuild tools first: (compat-libuv, libuv,) cmake, binutils, gcc49, m4, autoconf, automake
3. Rebuild libraries that have major version updated: such as compat-lib??? and lib???
4. Rebuild libraries that have minor version updated: such as sqlite, curl, tbb, ...
4. Rebuild other packages
