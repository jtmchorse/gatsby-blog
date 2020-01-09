---
template: "post"
draft: false
slug: "/posts/day-54/"
category: "100 Days of Code"
tags:
  - "Web Development"
  - "100daysofcode"
  - "Gatsby"
  - "Wordpress"
socialImage: ""
title: Day 54 
date: "2020-01-08"
description: "Udemy -Gatsby JS & Wordpress - Day 14 -Advanced custom field"
time: 
---

### Wordpress advanced custom fields

1 - install new plugin "ACF" - advanced custom fields

2 - install acf to rest api - so we can query the info into gatsby.

After these are installed, head to the new ACF setting menus in the Wordpress Admin UI. Screenshot to follow.

![Wordpress Advanced Custom Fields Admin UI Location](../../static/media/2020-01-09-Gatsby-wordpress-advanced-cutom-fields.png)

We will roughly follow these steps outlined below.

1. Add new field group in ACF - "Portfolio", 
2. call it portfolio url
3. type url
4. required
5. post-type = portfolio


![Wordpress Advanced Custom Fields Admin UI](../../static/media/2020-01-09-Wordpress-advanced-custom-fields-admin-ui.png)

Now inside the portfolio posts, there will be a new custom field with a "portfolio url" title. This is so we can show the url of the portfolio piece.


Restart gatsby, head to graphiql, edges, node acf portfoliourl !

![Advanced Custom Fields are now available in GraphiQL](../../static/media/2020-01-09-ACF-GraphiQL.png)

Next up, lets build that into Gatsby.


