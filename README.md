pipelight-selinux
=================

SELinux policy-module for pipelight.  This is intended to use with Fedora or
Fedora-EPEL.  Other distros using SELinux might work as well.

***

Changelog
---------

* 2014-07-14
  - v 0.1.0 -- initial module

***

Installation
------------

**On Fedora or Fedora-EPEL this gets automatically installed with pipelight.**

For manual installation or development:

```sh
git clone [git-repo-url] pipelight-selinux
cd pipelight-selinux
make -f /usr/share/selinux/devel/Makefile
install -p -m 644 -D pipelight.pp /usr/share/selinux/packages/pipelight/pipelight.pp
semodule -i /usr/share/selinux/packages/pipelight/pipelight.pp
```

***

License
-------

Copyright (c) 2014 Björn Esser <besser82@fedoraproject.org>
All rights reserved.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
