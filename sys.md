---
title: SYS ~~ Common Stuff
description: Here commons pieces of code for play around Linux System
published: true
date: 2019-11-25T14:34:13.394Z
tags: sys
---

# Header
Your content here

```
crontab -l -u Adminvas
du -khs *
ls -lrt
```

## tool
### ssh-add
https://www.cyberciti.biz/faq/unix-linux-appleosx-bsd-ssh-add-agent-command-set-lifetime/

```
#··· listing current loaded keys
ssh-add -l
ssh-add -L

#··· deleting specific key
ssh-add -d ~/.ssh/random_rsa
# deleting all the keys
ssh -D


#··· locking the agent -x
sh-add -x
#··· unlocking the agent -X
ssh-add -X

#··· lifetime set to 60 seconds (defaul)
#··· minutes ssh-add -t 30m
#··· hours ssh-add -t 30h
#··· days ssh-add -t 1d
#··· weeks ssh-add -t 2w
ssh-add -t 60  ~/.ssh/random_rsa
```


# HDMI status
```
[aa@localhost ~]$ cat /sys/class/drm/card0/*HDMI*/status
disconnected
[aa@localhost ~]$ cat /sys/class/drm/card0/*HDMI*/status
connected
```




