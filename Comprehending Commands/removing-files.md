## removing-files
using rm command 

**Flag:** 'pwn.college{Qgw1k3UlhYgy_qWFUoSzmdZPwks.QX2kDM1wSOwEzNzEzW}'

```
hacker@commands~removing-files:~$ touch delete_me
hacker@commands~removing-files:~$ ls
Desktop  c  delete_me  key  key.pub
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/run
bash: /challenge/run: No such file or directory
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{Qgw1k3UlhYgy_qWFUoSzmdZPwks.QX2kDM1wSOwEzNzEzW}

```

## What I Learned
This challenge create a delete_me file in your home directory, use rm to remove it, then run /challenge/check
