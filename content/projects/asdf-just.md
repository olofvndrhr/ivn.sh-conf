+++
title = "asdf-just"
description = "asdf plugin for just"
date = "2022-07-23"
type = ["default"]
+++

---

## asdf plugin for just

#### https://github.com/olofvndrhr/asdf-just

For my development and testing workflow I use the [asdf version manager](https://github.com/asdf-vm/asdf).
It lets you install multiple versions of the same tool at once and change the used version on the fly.

I also needed the tool [just](https://github.com/casey/just), which is like [make](https://www.gnu.org/software/make/),
but more for automation and less for compiling.

But as the current plugin for just was not working, i wrote my own one and created a [pull-request](https://github.com/asdf-vm/asdf-plugins/pull/629) for the official plugin
repository of asdf.
The [PR](https://github.com/asdf-vm/asdf-plugins/pull/629) was quickly merged, and now it is an official asdf plugin.
