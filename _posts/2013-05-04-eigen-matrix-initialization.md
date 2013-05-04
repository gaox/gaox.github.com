---
layout: post
title: "Eigen matrix initialization"
description: ""
category: 
tags: [Eigen]
---
{% include JB/setup %}

Eigen does `not` initialize the matrix elements as zero. This may introduce bugs when I want to use a diagonal matrix but only set the diagonal entires.
To set the matrix to zero, do this

    matrix.setZero();
