---
layout: post
title: "Automatically push to bitbucket"
description: ""
category: 
tags: []
---
{% include JB/setup %}

I wrote a crontab to automatically run `git commit` and `git push` to back up
my bitbucket pages. To push successfully I need to install `keychain` and run

`/usr/local/bin/keychain $HOME/.ssh/id_dsa`

Then add 

`source $HOME/.keychain/${HOSTNAME}-sh`

to my shell script.

