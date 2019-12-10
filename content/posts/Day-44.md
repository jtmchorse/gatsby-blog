---
template: "post"
draft: false
slug: "/posts/day-44/"
category: "100 Days of Code"
tags:
  - "Web Development"
  - "100daysofcode"
  - "Gatsby"
  - "Wordpress"
socialImage: ""
title: Day 44
date: "2019-12-09"
description: "Udemy -Gatsby JS & Wordpress - Day 4"
time: 
---

### Setting homepage

Destructure the createPages action object, [Gatsbyjs docs](https://www.gatsbyjs.org/docs/actions/#createRedirect)

I'm not certain that using a global redirect is really the best option. Say you have a redirect from `/` to `/home` that feels like bad practice. I've always seen a flicker on my local machine. Your mileage may vary, redirect with caution, or maybe use your .htaccess folder to redirect.
