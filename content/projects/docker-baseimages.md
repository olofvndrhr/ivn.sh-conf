+++
title = "docker baseimages"
description = "creating baseimages for deployment"
date = "2021-11-04"
type = ["default"]
+++

---

## Docker baseimages for app deployment

https://github.com/olofvndrhr/docker-baseimages

This is a relatively small project.

I thought, that if i deploy my apps with docker, then i should also create the base container for it. So i created a normal and a slim version. Both of them feature the [s6 overlay](https://github.com/just-containers/s6-overlay) and cron. The normal version also has some commonly used tools bundled with it.

S6 is really practical, because you can set the userid and groupid mappings via environment variables and the services are always under supervison.

```yml
  environment:
    - PUID=
    - PGID=
```