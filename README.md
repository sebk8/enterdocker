# enterdocker

"enterdocker" is a simple Shellskript that allows you to easily use 'nsenter' to get fast access to Docker or run commands.

`SYNTAX: enterdocker <dockername/dockerid> [exec command in docker]`

If you're going to execute a command directly over this script (or nsenter) please consider to specify absolute file paths:

```
# enterdocker myDocker ls --> WRONG
# enterdocker myDocker /bin/ls --> RIGHT
```

(NOTE: I didn't found a way to get a dockers $PATH for for the host ... I may fix this soon or anyone of you guys comes up with a good idea )



Copy the script somewhere where your $PATH variable destinates (e.g.: /usr/local/sbin/).
