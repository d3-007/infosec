## hidden-files
. operator is used for hidden files 

**Flag:** 'pwn.college{8o6V8VHM-6mZK46Qr_K_S-TSMzm.QXwUDO0wSOwEzNzEzW}'

```
hacker@commands~hidden-files:~$ ls -a
.   .ICEauthority  .cache   .dbus   Desktop  key
..  .bash_history  .config  .local  c        key.pub
hacker@commands~hidden-files:~$ ls
Desktop  c  key  key.pub
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.           .flag-5410355112146  challenge  home   lib64   mnt  proc  sbin  tmp
..          bin                  dev        lib    libx32  nix  root  srv   usr
.dockerenv  boot                 etc        lib32  media   opt  run   sys   var
hacker@commands~hidden-files:/$ .flag-5410355112146
bash: .flag-5410355112146: command not found
hacker@commands~hidden-files:/$ /.flag-5410355112146
bash: /.flag-5410355112146: Permission denied
hacker@commands~hidden-files:/$ cat .flag-5410355112146
pwn.college{8o6V8VHM-6mZK46Qr_K_S-TSMzm.QXwUDO0wSOwEzNzEzW}
hacker@commands~hidden-files:/$ 
```

## What I Learned
ls doesn't list all the files by default. Linux has a convention where files that start with a . don't show up by default in ls and in a few other contexts.
To view them with ls, you need to invoke ls with the -a flag
