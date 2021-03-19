---
layout: article
title: Git - Remove Garbage
date: 2021-03-19 11:03:14
tags:
---

More info: [Source](https://noteskeeper.ru/heritage/621/)

## Guide

### Remove all unused objects

``` bash
git gc
```
### Remove non-exist branches

``` bash
git remote prune origin
```
### Remove unreach commits

``` bash
git reflog expire --expire=1.minute refs/heads/development
git fsck –unreachable
git gc
```


