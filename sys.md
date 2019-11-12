---
title: SYS ~~ Common Stuff
description: Here commons pieces of code for play around Linux System
published: true
date: 2019-11-12T11:04:02.129Z
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

#···deleting specific key
ssh-add -d ~/.ssh/random_rsa
# deleting all the keys
ssh -D


#···locking the agent -x
sh-add -x
#···unlocking the agent -X
ssh-add -X

#···lifetime set to 60 seconds
ssh-add -t 60  ~/.ssh/random_rsa
```