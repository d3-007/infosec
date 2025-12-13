# level 2-3

### The password for the next level is stored in a file located in the home directory


```
bandit2@bandit:~$ ls
--spaces in this filename--
bandit2@bandit:~$ cat readme
cat: readme: No such file or directory
bandit2@bandit:~$ cat ./-
cat: ./-: No such file or directory
bandit2@bandit:~$ cat ./--spaces in this filename--
cat: ./--spaces: No such file or directory
cat: in: No such file or directory
cat: this: No such file or directory
cat: filename--: No such file or directory
bandit2@bandit:~$ cat "./--spaces in this filename--"
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
bandit2@bandit:~$ exit
logout
Connection to bandit.labs.overthewire.org closed.
```

## Commands used

1.ssh -p 2220 bandit2@bandit.labs.overthewire.org
2. ls
3. cat "./--spaces in this filename--"
4. exit
 

 
