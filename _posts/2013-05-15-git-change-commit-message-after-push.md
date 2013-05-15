---
layout: post
title: "git change commit message after push"
description: ""
category: 
tags: [git]
---
{% include JB/setup %}

From stackoverflow,

`git commit --amend -m "message"`

`git push --force`

Anyone already pulled needs to do

`git fetch origin`

`git reset --hard origin/master # Loses local commits`

