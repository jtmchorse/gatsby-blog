---
template: "post"
draft: false
slug: "/posts/day-53/"
category: "100 Days of Code"
tags:
  - "Web Development"
  - "100daysofcode"
  - "Gatsby"
  - "Wordpress"
socialImage: ""
title: Day 53 
date: "2020-01-06"
description: "Udemy -Gatsby JS & Wordpress - Day 13 - Custom page templates in Wordpress"
time: 
---

### Creating page templates

This happens inside the wordpress theme, in our case we are using the nearly blank theme provided by the author, "wp-gatsby-js-theme-starter" -> [Github](https://github.com/tomphill/wp-gatsby-js-theme-starter).

We then need to add a new php file, we are calling that "portfolio_under_content" for this exercise.

Essentially we are using this new file so that in the future we can tell Gatsby which template we should use for that type of page. Wordpress will continue to not do any styling.

After the new php file is saved, and we verify it works inside the Wordpress admin webpage, we'll need to update `gatsby-node.js` to have a path.resolve variable. We will also need to update our "All wordpressPage" query, so that it includes the template option.

This variable will be how we tell Gatsby which page template to use.

Finally in our `createPage` function we'll need to add an if statement, that way we can give the basic page template to any page `template` type that is page, or the 'portfolio_under_content' template to those pages which come from Wordpress with that temple chosen. We are the ones who choose that in the Wordpress admin section.
