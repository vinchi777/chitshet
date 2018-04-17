### Tailing a process 

```
cd /proc/{process-id}
Then look for the fd directory underneath

$ cd fd
This fd directory hold the file-descriptors objects that your program is using (0: stdin, 1: stdout, 2: stderr) and just tail -f the one you need - in this case, stdout):

$ tail -f 1
```
