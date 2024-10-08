# An Epic Filesystem Quest
In this challenge we use all the previously learnt commands like `cd`, `ls`, `cat` etc to follow the flag hunt.
```
Connected!
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
DOSSIER  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin      challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat DOSSIER
Great sleuthing!
The next clue is in: /opt/aflplusplus/nyx_mode/QEMU-Nyx/hw/virtio

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/aflplusplus/nyx_mode/QEMU-Nyx/hw/virtio
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/QEMU-Nyx/hw/virtio$ ls
Kconfig               vhost-user-fs-pci.c     virtio-9p-pci.c          virtio-input-pci.c  virtio-rng-pci.c
Makefile.objs         vhost-user-fs.c         virtio-balloon-pci.c     virtio-mmio.c       virtio-rng.c
SNIPPET               vhost-user-input-pci.c  virtio-balloon.c         virtio-net-pci.c    virtio-scsi-pci.c
trace-events          vhost-user-scsi-pci.c   virtio-blk-pci.c         virtio-pci.c        virtio-serial-pci.c
vhost-backend.c       vhost-user.c            virtio-bus.c             virtio-pci.h        virtio.c
vhost-scsi-pci.c      vhost-vsock-pci.c       virtio-crypto-pci.c      virtio-pmem-pci.c
vhost-stub.c          vhost-vsock.c           virtio-crypto.c          virtio-pmem-pci.h
vhost-user-blk-pci.c  vhost.c                 virtio-input-host-pci.c  virtio-pmem.c
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/QEMU-Nyx/hw/virtio$ cat SNIPPET
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/arch/xtensa/kernel/syscalls

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/QEMU-Nyx/hw/virtio$ cd /opt/linux/linux-5.4/arch/xtensa/kernel/syscalls
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/xtensa/kernel/syscalls$ ls -a
.  ..  .REVELATION  Makefile  syscall.tbl  syscallhdr.sh  syscalltbl.sh
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/xtensa/kernel/syscalls$ cat .REVELATION
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/Documentation/w1
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/xtensa/kernel/syscalls$ cd /opt/linux/linux-5.4/Documentation/w1
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/w1$ ls
WHISPER  index.rst  masters  slaves  w1-generic.rst  w1-netlink.rst
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/w1$ cat WHISPER
Lucky listing!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/feature/logread/reduced

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/w1$ cd /opt/busybox/busybox-1.33.2/include/config/feature/logread/reduced
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/logread/reduced$ ls
LEAD  locking.h
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/logread/reduced$ cat LEAD
Great sleuthing!
The next clue is in: /opt/aflplusplus/frida_mode/test/png/persistent/hook

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/logread/reduced$ cd /opt/aflplusplus/frida_mode/test/png/persistent/hook
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/frida_mode/test/png/persistent/hook$ ls
GNUmakefile  INSIGHT  Makefile  cmodule.js  load.js
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/frida_mode/test/png/persistent/hook$ cat INSIGHT
Great sleuthing!
The next clue is in: /usr/share/R/share/licenses

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/frida_mode/test/png/persistent/hook$ cat /usr/share/R/share/licenses/ALERT-TRAPPED
Tubular find!
The next clue is in: /opt/aflplusplus/qemu_mode/qemuafl/target/rx
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/frida_mode/test/png/persistent/hook$ cd /opt/aflplusplus/qemu_
mode/qemuafl/target/rx
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/target/rx$ ls
NOTE         cpu-qom.h  cpu.h    gdbstub.c  helper.h      meson.build  translate.c
cpu-param.h  cpu.c      disas.c  helper.c   insns.decode  op_helper.c
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/target/rx$ cat NOTE
Great sleuthing!
The next clue is in: /usr/share/locale/pt_BR/LC_MESSAGES

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/target/rx$ cd /usr/share/locale/pt_BR/LC_MESSAGES
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/pt_BR/LC_MESSAGES$ ls -a
.   .MEMO   dpkg.mo  iso_15924.mo   iso_3166-3.mo  iso_4217.mo   iso_639-3.mo  iso_639_3.mo      nvim.mo
..  apt.mo  fish.mo  iso_3166-1.mo  iso_3166.mo    iso_639-2.mo  iso_639.mo    libapt-pkg6.0.mo  sphinx.mo
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/pt_BR/LC_MESSAGES$ cat .MEMO
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{QgFLZ7E9jfCxfmBaEXzKN8wgfqo.dljM4QDLzIzN0czW}
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/pt_BR/LC_MESSAGES$
```
