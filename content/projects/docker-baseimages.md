+++
title = "docker baseimages"
description = "creating baseimages for deployment"
date = "2021-11-04"
type = ["default"]
+++

---

## Docker baseimages for app deployment

#### https://github.com/olofvndrhr/docker-baseimages

This is a relatively small project.

I thought, that if I deploy my apps with docker, then I should also create the base container images for it.
So I created a normal and slim version.
Both of them feature the [s6 supervisor](https://github.com/just-containers/s6-overlay) and cron.
The normal version also has some commonly used tools bundled with it.

S6 is really practical, because you can map the UID and GID of every service you run in your container.
Also, the services are always supervised, so they will restart if they fail.

Later I also added a base version without the [s6 supervisor](https://github.com/just-containers/s6-overlay)
for use cases which don't require supervision of the application.

> Snippet to map the UID and GID for the default user `abc` in a docker-compose file
```yml
  environment:
    - PUID=
    - PGID=
```
