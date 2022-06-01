+++
title = "flox-dockerized"
description = "Dockerization of flox"
date = "2022-04-16"
type = ["default"]
+++

---

## Dockerization of flox

#### https://github.com/olofvndrhr/flox-dockerized

Flox is a personal watchlist, written in php.

Before I created my version, I used a docker container of flox from another user (I can't remember which one).

But this version did not have a supervisor installed, so I created my own docker container for it with supervision.

The baseimage for the flox container is the [debian-s6](https://github.com/olofvndrhr/docker-baseimages) image from myself.
It includes everything needed.

I also built it for arm64 and amd64, so it can even run on raspberry pi's or other arm processors.

> The original repository: [devfake/flox](https://github.com/olofvndrhr/docker-baseimages)
