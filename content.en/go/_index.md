---
weight: 3
bookFlatSection: true
title: "2. Introduction to Go"
bookCollapseSection: true
---

# Introduction to Go

The single most important thing before doing anything: *installing Go*. The process is relatively simple, the documentation provided by the [official site](https://go.dev/doc/install) it's enough for most cases.

Just choose a specific OS and follow the instructions. If, for some reason the steps are not enough:

## Windows

1. For Windows I recommend this blog by Handhika Yanuar Pratama for installation: https://handhikayp.medium.com/golang-101-installing-golang-for-your-windows-environment-6b82c588fa40
2. And then following the official site's Tutorial: https://go.dev/doc/tutorial/getting-started

## Linux

```sh
# latest release at moment of writing
curl -O https://go.dev/dl/go1.24.5.linux-amd64.tar.gz
rm -rf /usr/local/go && tar -C /usr/local -xzf go1.24.5.linux-amd64.tar.gz
export PATH=$PATH:/usr/local/go/bin # add this in .bashrc / .zshrc
```

[> Next](/go/hello_world)
