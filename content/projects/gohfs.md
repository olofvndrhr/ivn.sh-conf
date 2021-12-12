+++
title = "gohfs - docker"
description = "Dockerization of gohfs"
date = "2021-06-07"
type = ["default"]
+++

---

## Dockerization of gohfs

https://github.com/olofvndrhr/gohfs

To be deployed in my environment i needed this application in a containerized format. But the original developer did not have a container for it yet. So i created one with the [s6 overlay](https://github.com/just-containers/s6-overlay) for easy usermapping and failure detection.
The pull request with the changes was accepted and can also be viewed at the [original repository](https://github.com/finzzz/gohfs).

