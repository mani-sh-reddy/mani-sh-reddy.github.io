---
layout: post
title: "recursive git pull"
description: ""
comments: false
keywords: ""
color: ""
---

```bash
find . \
-maxdepth 1 \
-type d \
-print \
-execdir git \
--git-dir={}/.git \
--work-tree=$PWD/{} pull origin main \;
```
