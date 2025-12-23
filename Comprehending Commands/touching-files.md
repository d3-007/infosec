## touching-files
to create a file within the directory 

**Flag:** 'pwn.college{Eg3uDpC3AFSVo9B0QT71nHZo6gI.QXwMDO0wSOwEzNzEzW}'

```
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.2dyEZcT2Od
hacker@commands~touching-files:/tmp$ cd /pwn
bash: cd: /pwn: No such file or directory
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{Eg3uDpC3AFSVo9B0QT71nHZo6gI.QXwMDO0wSOwEzNzEzW}

```

## What I Learned
create a new, blank file by touching it with the touch command after going into the tmp directory 
