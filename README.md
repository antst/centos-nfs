centos-nfs
==========

Kernel NFS module from Centos/RHEL, with few patches/fixes, prepared as DKMS module

Applied patches:

1) patch to handle access to  exec-only files in right way. Backported from 3.1.x kernels

#Installation

On target host perform next commands (assuming that you already have installed dkms)

```bash
 git clone https://github.com/antst/centos-nfs.git /usr/src/nfs-358.11.1
 dkms install -m nfs -v 358.11.1
 ```
 
 native module will be masked by this one.
 



