# Background Processes Tasks

1. By using vim **create** a text file, then **suspend** vim in the background.
2. With **jobs** command **verify** that **vim** is suspended in the background.
3. Run **find / > /tmp/systemfiles.txt** 2>/dev/null in the foreground, then **suspend** it in the background before it finishes.
5. **Start** four long sleep processes in background.
6. **Display** only the sleep jobs in the background.
7. Use **kill** command to suspend the last two sleep processes.
8. **Continue** the find process in the background (make sure it runs again). 
9. **Put** one of the sleep commands back in foreground.


# Bounce question
- Explain in details why the result is different for each command in the below code snippet.

```shell

root@server# echo $$ $PPID
89 0
root@server# bash -c "echo $$ $PPID"
89 0
root@server# bash -c 'echo $$ $PPID'
350 89
root@server# bash -c `echo $$ $PPID`
0: 89: command not found
```
