+++
title = "powerdns for arm64"
description = "powerdns containers for arm64"
date = "2024-01-27"
type = ["default"]
+++

---

## powerdns containers for arm64

#### https://github.com/olofvndrhr/docker-pdns

> The whole powerdns suite for arm64+amd64.

The official docker builda from [powerdns](https://github.com/PowerDNS/pdns) only include the amd64 version, but as i was planning on using them on some arm64 machine I needed a compatible image.

So the easy to maintain way was to:

1.  create new build scripts
2.  build the images for amd64 and arm64
3.  publish them on the official container repository

And as I was also using lightningstream for replication purposes, it was also included in the build.
The final repository then contained builds with sample configs for:

-   [PowerDNS Authoritative Nameserver](https://doc.powerdns.com/authoritative/)
-   [PowerDNS Recursor](https://doc.powerdns.com/recursor/)
-   [Powerdns Lightningstream](https://doc.powerdns.com/lightningstream/)
