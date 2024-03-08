---
title: git-submodule
date: 2024-03-08 02:09:43
tags:
- Git
---
## Submodule

### Add Submodule

```bash
git submodule add <repository> <path>
```

Example:

```bash
git submodule add https://github.com/probberechts/hexo-theme-cactus.git themes/cactus
```

### Clone repository with submodule

如果是 repository 早已有 submodule 的情況下，clone 下來的 submodule 正常情況下會是空的

```bash
git clone https://github.com/Chengxufeng1994/hexo-site
```

需要下以下兩個指令:

1. `git submodule init`
2. `git submodule update`

也可以透過 flag 同時初始化和下載:

1. `git submodule update --init --recursive`

### Clone repository with submodule (init/update)

```bash
git clone --recurse-submodules https://github.com/Chengxufeng1994/hexo-site
```

### Remove Submodule

```bash
git rm <submodule_name>
```
