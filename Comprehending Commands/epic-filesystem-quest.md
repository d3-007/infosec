## epic-filesystem-quest
Your first clue is in /. Head on over there.
Look around with ls. There'll be a file named HINT or CLUE or something along those lines!
cat that file to read the clue!Depending on what the clue says, head on over to the next directory (or don't!).
Follow the clues to the flag!

**Flag:** 'pwn.college{kLMW5d4d-_DCgEeJsklfidB3p7C.QX5IDO0wSOwEzNzEzW}'

```
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
HINT  bin  boot  challenge  dev  etc  flag  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@commands~an-epic-filesystem-quest:/$ cat HINT
Congratulations, you found the clue!
The next clue is in: /usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/third_party/2and3/cryptography/hazmat

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/third_party/2and3/cryptography/hasmat
ls: cannot access '/usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/third_party/2and3/cryptography/hasmat': No such file or directory
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/third_party/2and3/cryptography/hazmat
DISPATCH-TRAPPED  __init__.pyi  backends  bindings  primitives
hacker@commands~an-epic-filesystem-quest:/$ cat DISPATCH-TRAPPED
cat: DISPATCH-TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/third_party/2and3/cryptography/hazmat/DISPATCH-TRA
PPED
Yahaha, you found me!
The next clue is in: /usr/share/racket/pkgs/plai-doc/compiled

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/racket/pkgs/plai-doc/compiled 
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/plai-doc/compiled$ ls -a
.  ..  .NUGGET  info_rkt.dep  info_rkt.zo
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/plai-doc/compiled$ cat .NUGGET
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/include/config/init/env
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/plai-doc/compiled$ cd /opt/linux/linux-5.4/include/config/init/env
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/init/env$ ls
CUE  arg
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/init/env$ cat CUE
Great sleuthing!
The next clue is in: /usr/local/lib/python3.8/dist-packages/outcome

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/init/env$ ls /usr/local/lib/python3.8/dist-packages/outcome
DOSSIER-TRAPPED  __init__.py  __pycache__  _impl.py  _util.py  _version.py  py.typed
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/init/env$ cat /usr/local/lib/python3.8/dist-packages/outcome/DOSSIER-TRAPPED
Great sleuthing!
The next clue is in: /usr/share/javascript/mathjax/localization/bg

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/init/env$ cd /usr/share/javascript/mathjax/localization/bg
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/localization/bg$ ls -a
.  ..  .EVIDENCE  FontWarnings.js  HTML-CSS.js  HelpDialog.js  MathML.js  MathMenu.js  TeX.js  bg.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/localization/bg$ cat .EVIDENCE
Congratulations, you found the clue!
The next clue is in: /usr/lib/x86_64-linux-gnu/perl/5.30.0/auto/ODBM_File

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/localization/bg$ cd /usr/lib/x86_64-linux-gnu/perl/5.30.0/auto/ODBM_File
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl/5.30.0/auto/ODBM_File$ ls -a
.  ..  .INSIGHT  ODBM_File.so
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl/5.30.0/auto/ODBM_File$ cat .INSIGHT
Tubular find!
The next clue is in: /opt/linux/linux-5.4/arch/ia64/oprofile

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl/5.30.0/auto/ODBM_File$ cd /opt/linux/linux-5.4/arch/ia64/oprofile
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/ia64/oprofile$ ls -a
.  ..  Makefile  POINTER  backtrace.c  init.c  perfmon.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/ia64/oprofile$ cat POINTER
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/arch/arm/mach-pxa/include

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/ia64/oprofile$ cd /opt/linux/linux-5.4/arch/arm/mach-pxa/include
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-pxa/include$ ls -a
.  ..  CLUE  mach
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-pxa/include$ CLUE
bash: CLUE: command not found
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-pxa/include$ cat CLUE
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{kLMW5d4d-_DCgEeJsklfidB3p7C.QX5IDO0wSOwEzNzEzW}
```


