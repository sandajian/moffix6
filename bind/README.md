#bind

##Compiled from
<pre>bind-9.11.0-4.P1.fc26.src.rpm</pre>

##Modified
<pre>
- Added 2 files from bind-9.8.4-3.P1: named.NetworkManager, named.init
- Modified systemd-related lines to sysvinit-related
- Requires: python3 -> python34, libdb-devel -> db4-devel
- Removed 'sdb-chroot'
- /run/named -> /var/run/named
- Modified default /etc/named.conf: /run/named -> /var/run/named, comments out the 'crypto-policies' line.
</pre>
