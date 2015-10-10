# vmware-kernel-patches
Kernel patches for VMWare Linux Guest
Combination of VMWare Photon patches + my own stuff

# Usage on Debian
* Grab 4.2.X from kernel.org
* Patch the tree (eg `for p in *.patch; do patch -p1 < $p; done`)
* move config to .config in the tree
* make oldconfig (eg `yes "" | make oldconfig`)
* build the normal way (eg `make-kpkg ......... linux-image linux-headers`)
* install
