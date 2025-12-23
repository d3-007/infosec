## comparing-files
how to use diff command 

**Flag:** 'pwn.college{gWbUFPqATB6kcbpIeBEM5T-TMWF.01MwMDOxwSOwEzNzEzW}'

```
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
37a38
> pwn.college{gWbUFPqATB6kcbpIeBEM5T-TMWF.01MwMDOxwSOwEzNzEzW}
```

## What I Learned
In this challenge, diff compares two files line by line and shows you exactly what's different between them
37a38 also shows where the disparrity occours and > tell us which text has disparity.
