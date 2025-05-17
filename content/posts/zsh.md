---
title: "Setting up zsh"
date: 2021-09-07
draft: false
author: Nic 
description: Setting up zsh consistently. Assuming zsh is installed…
categories:
    - tech
---

### Note to self

Setting up zsh consistently. Assuming zsh is installed…

#### Install oh-my-zsh

```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```


#### Install zsh-autosuggestions and zsh-syntax-highlighting

```
cd ~/oh-my-zsh/custom/plugins
git clone https://github.com/zsh-users/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
```

#### Configure

* delete the block setting `EDITOR` and replace with `export EDITOR=vim`
* set the `plugins` list to `(zsh-autosuggestions zsh-syntax-highlighing vi-mode git redis-cli)`