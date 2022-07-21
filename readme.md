# Today


Okay it's 2022 and you still don't want to run nepomunk, a holistic semantic
filesystem approach never happened and you're stuck with a million files in
your Download folder, home folder etc.

So I use this script to give me a nice work environment, based on each day.

Every time you open bash, it'll drop you into today's directory. 

When I think about stuff it's like.. oh yeah I worked on that last week, last
year, etc - the folder structure makes this a lot easier, and you can just write
'notes' or 'meeting-with-joe' and you know the ref date.

For your bashrc:
```
alias t='source /path/to/today'

t
```

Now every day you'll know what you worked on yesterday!

```
# this is where you'll get dropped by default.
calvin@bison:~/work/2022/07/10$ 

calvin@bison:~/work/2022/07/10$ ls
WardsPerlSimulator.pl

calvin@bison:~/work/2022/07/10$ cd ..; ls;
01  02  04  05  06  07  08  09  10

calvin@bison:~/work/2022/07$ cd ..; ls
01  02  03  04  05  06  07
calvin@bison:~/work/2022$ cd ..; ls
2021  2022
```

additionally you'll get a shortcut, you can type 't' as a bash fn, or go to ~/t/
which is symlinked and updated everytime you run today (which is everytime you
open bash or hit 't'. this is useful if you want to have Firefox/Slack/whatever
always save something in your 'today' folder.
