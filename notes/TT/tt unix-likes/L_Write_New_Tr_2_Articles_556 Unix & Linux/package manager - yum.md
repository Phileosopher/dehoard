
[Vivek Gite](https://www.cyberciti.biz/faq/centos-redhat-fedora-yum-lock-package-version-command/)
CentOS / RHEL: Yum Lock Package Version At a Particular Version

[Linux Stack Exchange](https://unix.stackexchange.com/questions/259640/how-to-use-yum-to-get-all-rpms-required-for-offline-use)
How to use yum to get all RPMs required, for offline use?

[Red Hat Customer Portal](https://access.redhat.com/solutions/10154)
How to use yum to download a package without installing it

[CentOS Wiki](https://wiki.centos.org/TipsAndTricks/YumAndRPM)
Yum and RPM Tips and Tricks

[Computer Hope](https://www.computerhope.com/unix/yum.htm)
yum command help + examples

[David Newcomb](http://www.bigsoft.co.uk/blog/2012/01/06/rpmdb-unable-to-join-the-environment)
(2012) yum install failing on `rpmdb: unable to join the environment` or `db3 error(11) from dbenv->open: Resource temporarily unavailable`. Do the followings:
```
rm -rf /var/lib/rpm/__db*
rpm --rebuilddb
```

[Benjamin Cane](https://bencane.com/2013/12/23/yum-plugins-verifying-packages-and-configurations-with-yum-verify/)
(2013) Yum Plugins: Verifying packages and configurations with Yum Verify
