---
title: Install Jekyll and a custom theme on WLS2
tags: jekyll
license: false
---

Showcase of how to install Jekyll and a custom theme on WSL2.

<!--more-->

## Install WSL2

## Install Jekyll

Install Ruby and other requirements.

```shell
sudo apt-get install ruby-full build-essential zlib1g-dev
```

Configure ```.bashrc``` so that the gems will be installed to the home directory.

```shell
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

Install jekyll and bundler.

```shell
gem install jekyll bundler
```