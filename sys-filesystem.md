---
title: SYS ~~ filesystem
description: linux filesystem and storage stuff
published: true
date: 2019-11-07T13:24:40.838Z
tags: sys, sys-filesystem
---

# Header
Your content here

## tool
### du ~~ disk usage

```
# essentials
du -khs *

```

### du ~~ disk usage

```
# only display df lines that have more fs usage than 80%
df -P | awk '0+$5 >= 80 {print}'

```

### ls ~~ list

```
# essentials
ls -lrt
ls -al
```
