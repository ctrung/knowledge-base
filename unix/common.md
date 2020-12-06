# Unix common commands

## execution trace

```console
$ sh -x -c 'who | wc -l'
+ who
+ wc -l
1
```

In a shell script
```console
#! /bin/sh

set -x      # activate trace
echo hello

set +x      # deactivate trace
echo world
```

## stty (set terminal)

```console
$ stty -echo    # deactivate echo
$ stty echo     # activate echo
```

## tr (translate, transliterate)

```console
$ echo hello | tr 'elo' 'apy'               # replace corresponding elements
happy
```

```console
$ tr -d '\r' < dos-file.txt > unix-file.txt # remove carriage returns
```
