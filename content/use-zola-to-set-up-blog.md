+++
title = "Set up your blog with zola"
date = 2022-01-09T18:18:18+08:00

[taxonomies]
tags = ["Rust"]

+++

> zola is a fast static site generator in a single binary with everything built-in. This article is about how to build a blog in Github Pages with zola

---

## Initialize your blog
### Install zola  
I use WSL on Windows 10, with Homebrew as a package manager, and the install command is: 

```
brew install Zola
```

### Initialize a directory

use `zola init` command to initialize a directory

```bash
zola init blog
```

## Install theme
### Go to theme directory

```
cd blog/themes
```

### Clone the theme you want
```
git clone https://github.com/carpetscheme/lightspeed.git
```

### Config in config.toml

```toml
theme="lightspeed"
```

### Auto CI/CD

See official doc: *[传送门](https://www.getzola.org/documentation/deployment/github-pages/)*

## Conclusion 🐱
Pros:
- Easy to install
- All in one binary
- Fast

Cons:
- Not that many theme 
- Template syntax is a little bit confusing

