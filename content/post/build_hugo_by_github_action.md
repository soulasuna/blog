---
title: "Build Hugo By GitHub Action"
date: 2023-01-27T23:09:12+08:10
draft: false
---

# Build Hugo By GitHub Action
> Take macOS for example.

## Front Environmental Conditions
1. Install Git
2. Install Go version 1.18 or later

## Install Hugo And Config

1. install
```shell
brew install hugo;
```
2. test
```shell
hugo version;
```

3. new site
```shell
hugo new site {name}
```

4. themes
> Take `m10c` for example.

```shell
git clone https://github.com/vaga/hugo-theme-m10c.git themes/m10c
```

5. configration
```shell
echo "theme = 'm10c'" >> config.toml
```

6. post
```shell
hugo new post/{file name}.md
```

7. preview
```shell
hugo server -D
```

## Build By Github Action

TODO

