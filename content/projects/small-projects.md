+++
title = "small projects"
description = "list of a few small projects"
date = "2024-01-01"
type = ["default"]
+++

---

## Dockerization of gohfs

#### https://github.com/olofvndrhr/gohfs

To be deployed in my environment I needed this application in a containerized format.
But the original developer did not have a container for it yet.

So I created one with the [s6 supervisor](https://github.com/just-containers/s6-overlay) for easy user mapping and failure detection.

The pull request with the changes was accepted and can also be viewed at the [original repository](https://github.com/finzzz/gohfs).

## Dockerization of flox

#### https://github.com/olofvndrhr/flox-dockerized

Flox is a personal watchlist, written in php.

Before I created my version, I used a docker container of flox from another user (I can't remember which one).

But this version did not have a supervisor installed, so I created my own docker container for it with supervision.

The baseimage for the flox container is the [debian-s6](https://github.com/olofvndrhr/docker-baseimages) image from myself.
It includes everything needed.

I also built it for arm64 and amd64, so it can even run on raspberry pi's or other arm processors.

> The original repository: [devfake/flox](https://github.com/olofvndrhr/docker-baseimages)

## Improvements to a Lets Encrypt bash script

#### https://github.com/olofvndrhr/dehydrated-hook-cloudflare

I changed the script to fit my needs.
In the process I removed one package dependency and increased readability of the script.
