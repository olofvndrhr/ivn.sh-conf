+++
title = "manga-dlp"
description = "Manga download script in python3"
date = "2021-12-22"
type = ["default"]
+++

---

## Manga download script written in python3

#### https://github.com/olofvndrhr/manga-dlp

I was in search of a script to download multiple mangas at the same time without any interactive elements which require your attention.
The best I found was [mangadex-dl](https://github.com/frozenpandaman/mangadex-dl)
which didn't include multiple mangas, or all chapters at the same time.
So I took inspiration from mangadex-dl and wrote a script myself.
It includes all my needs and is extendable for other sites too.

I also created a docker container for it, built on my own base images.

> More infos are available in the [README.md](https://github.com/olofvndrhr/manga-dlp/blob/master/README.md)
> or for [docker](https://github.com/olofvndrhr/manga-dlp/blob/master/docker/README.md)

Features (summary):
* Multiple mangas via a file with links
* Ability to download all chapters available
* Save as zip, cbz, pdf or folder
* Add volume information
* Select language
