pipelight-selinux
=================

Description
-----------

SELinux policy-module for pipelight.  This is intended to use with Fedora or
Fedora-EPEL.  Other distros using SELinux might work as well.

***

Installation
------------

**On Fedora or Fedora-EPEL this gets automatically installed with pipelight.**

For manual installation or development:

```sh
git clone [git-repo-url] pipelight-selinux
cd pipelight-selinux
make -f /usr/share/selinux/devel/Makefile
install -p -m 0644 -D pipelight.pp /usr/share/selinux/packages/pipelight/pipelight.pp
semodule -i /usr/share/selinux/packages/pipelight/pipelight.pp
```
