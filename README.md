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

***

License
-------

    pipelight-selinux -- SELinux-based rules for pipelight
    Copyright (c) 2014 - 2015  Björn Esser  <besser82@fedoraproject.org>

    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License along
    with this program; if not, write to the Free Software Foundation, Inc.,
    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
