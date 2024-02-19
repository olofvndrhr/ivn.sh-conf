+++
title = "manga-dlp"
description = "Manga download script in python3"
date = "2022-07-25"
type = ["default"]
+++

---

## Manga downloader written in python3

#### https://github.com/olofvndrhr/manga-dlp

I was in search of a script to download multiple mangas at the same time without any interactive elements which require your attention.
The best I found was [mangadex-dl](https://github.com/frozenpandaman/mangadex-dl)
which didn't include multiple mangas, or all chapters at the same time.
So I took inspiration from mangadex-dl and wrote a script myself.
It includes all my needs and is extendable for other sites too.

I also created a docker container for it, built on my own base-image.

> More infos are available on the official docs: https://manga-dlp.ivn.sh/

**Feature summary:**

-   Multiple mangas via a file with links
-   Ability to download all chapters available
-   Save as zip, cbz, cbr, pdf or folder
-   Add metadata via the [comicinfo](https://anansi-project.github.io/docs/comicinfo/schemas/v2.0) format
-   Multi-language support
-   Volume support
-   Custom event hooks
-   [Docker image](https://hub.docker.com/repository/docker/olofvndrhr/manga-dlp)
-   [PyPi package](https://pypi.org/project/manga-dlp/)
-   etc.
