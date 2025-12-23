# Position yet elsewhere 
The challenge requires you to navigate trough files by using the keyword cd as a command and passing a path as its argument.

## My Solve
**Flag:** 'pwn.college{wDSjjC7bKcbWI5q6H8XRkb3aZiQ.QX4QTN0wSOwEzNzEzW}'


```
hacker@paths~position-elsewhere:~$ /
bash: /: Is a directory
hacker@paths~position-elsewhere:~$ cd /home
hacker@paths~position-elsewhere:/home$  /challenge/run
Incorrect...
You are not currently in the /var directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:/home$ cd /var
hacker@paths~position-elsewhere:/var$  /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Moving on to level 3
Please use the `cd` utility to change directory to /usr/share/build-essential
hacker@paths~position-elsewhere:/var$ ^C
hacker@paths~position-elsewhere:/var$ cd /usr/share/build-essential
hacker@paths~position-elsewhere:/usr/share/build-essential$  /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Moving on to level 4
Please use the `cd` utility to change directory to /var/log
hacker@paths~position-elsewhere:/usr/share/build-essential$ cd /var/log
hacker@paths~position-elsewhere:/var/log$  /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Moving on to level 5
Please use the `cd` utility to change directory to /
hacker@paths~position-elsewhere:/var/log$ cd /
hacker@paths~position-elsewhere:/$  /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{wbF168Du3VYHBoE8OTzwi6Hzr4S.QX3QTN0wSOwEzNzEzW}
```

## What I Learned
The correct directory was given in the challenge instructions when you run /challenge/run from the wrong location, which will give the right directory.
The given file was in the /proc/144/fd direcotry file and i had to change the path of the directory by passing a command cd and argument /proc/144/fd which took the control line to home page from where the files was accessed.
/challenge/run is an absolute path, invoked from the right directory after changing the directory.

## References
None.
'
