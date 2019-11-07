---
title: SYS ~~ filesystem
description: linux filesystem and storage stuff
published: true
date: 2019-11-07T19:44:53.041Z
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

### tar

```
# compress
tar -czvf name-of-archive.tar.gz /path/to/directory-or-file

# extract
tar -xzvf archive.tar.gz

```