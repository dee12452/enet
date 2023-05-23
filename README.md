# Enet for Vita

Code forked from https://github.com/lsalzman/enet
<br>
Vita net code copied from https://github.com/xyzz/vita-enet

## Vita Enet install instructions

Use the below method for installing enet into your VITASDK libraries.
<br>
<strong>NOTE: You *must* have the VITASDK / toolchain installed as a prerequisite.</strong>
<br>
```
$ mkdir build && cd build && cp ../VITABUILD .
$ vita-makepkg
...
$ libtool --finish "$VITASDK/arm-vita-eabi/lib"
$ vdpm ./enet-<version>-arm.tar.xz
```
<br>
This will install the latest version of the library.
To pin to a specific git commit, change the gitrev in the VITABUILD appropriately.

## See below for original readme

Please visit the ENet homepage at http://sauerbraten.org/enet/ for installation
and usage instructions.

If you obtained this package from github, the quick description on how to build
is:

\# Generate the build system.

autoreconf -vfi

\# Compile and install the library.

./configure && make && make install


