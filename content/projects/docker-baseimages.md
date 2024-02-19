+++
title = "docker baseimages"
description = "creating baseimages for deployment"
date = "2021-11-04"
type = ["default"]
+++

---

## Docker base-mages for container deployments

> the code for this project is hosted on my private gitea instance

This is a relatively small project.

As i deploy quite a few containers myself, some of them eventually have be customized.
For this use case i created my own base-image, to have a common starting point.
The image uses the [s6 supervisor](https://github.com/just-containers/s6-overlay) and already has cron installed.
It also has some commonly used tools bundled with it. So a perfect image for my use cases.

The S6 supervisor is also really practical, because you can map the UID and GID of every service you run in your container.
And the services are always supervised, so they will restart if they fail.

Later i created some more variants of the image, one without `s6`, one with `nginx` preinstalled and one with `nginx+php`.

> `compose.yml` snippet to map the UID and GID for the default user `abc` in a docker-compose file

```yml
environment:
    - PUID=
    - PGID=
```
