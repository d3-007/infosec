## grepping-for-a-needle-in-a-haystack
In this challenge,a hundred thousand lines of text into the /challenge/data.txt file.
grep it for the flag!

**Flag:** 'pwn.college{cfsLxkJFgb06j5RVX2EEqfy8hqS.QX3EDO0wSOwEzNzEzW}'

```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep SEARCH_STRING pwn.college
grep: pwn.college: No such file or directory
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep SEARCH_STRING /challenge/data.txt
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep SEARCH_STRING /challenge/data
grep: /challenge/data: No such file or directory
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{cfsLxkJFgb06j5RVX2EEqfy8hqS.QX3EDO0wSOwEzNzEzW}
```

## What I Learned
Grep will search the file for lines of text containing pwn.college and print them to the console.

