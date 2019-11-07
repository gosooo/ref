---
title: sre-docker
description: Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers
published: true
date: 2019-11-07T14:30:14.070Z
tags: sre, sre-docker
---

# Header
Your content here

http://crosbymichael.com/advanced-docker-volumes.html



How to use an entrypoint script to initialize container data at runtime


create a `vi docker-entrypoint.sh`

```
#!/bin/bash
set -e

if [ "$1" = 'postgres' ]; then
    chown -R postgres "$PGDATA"

    if [ -z "$(ls -A "$PGDATA")" ]; then
        gosu postgres initdb
    fi

    exec gosu postgres "$@"
fi

exec "$@"
```

add it `vi Dockerfile`

```
FROM debian:stretch
...
COPY docker-entrypoint.sh /usr/local/bin/
RUN ln -s /usr/local/bin/docker-entrypoint.sh / # backwards compat
ENTRYPOINT ["docker-entrypoint.sh"]
CMD ["postgres"]
```



[link-001] : https://success.docker.com/article/use-a-script-to-initialize-stateful-container-data