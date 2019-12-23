---
template: "post"
draft: false
slug: "/posts/day-51/"
category: "100 Days of Code"
tags:
  - "Web Development"
  - "100daysofcode"
  - "Gatsby"
  - "Wordpress"
socialImage: ""
title: Day 51 
date: "2019-12-22"
description: "Udemy -Gatsby JS & Wordpress - Day 11 - Custom post types"
time: 
---

### Custom post types

Today is a first for me, I have never before made a custom post type in wordpress. I have mucked about with the functions.php files before. If memory serves it was to do something with the WP thumbnails for a friend..

In this lesson we created a _Portfolio_ post type, after all this is a portfolio website we are building.

Here in an interesting [write up on Wordpress post types, along with custom posts](https://kinsta.com/blog/wordpress-custom-post-types/).

A few things we'll need to remember for rendering anything new from Wordpress in Gatsby.

1. We need to define new types in gatsby-config.js under the _includedRoutes_ block.

2. We need to include a GraphQL query inside gatsby-node.js.

3. We need to define the template that, in this case, the portfolio posts will be using. Luckily in our gatsby-node file we already did this for Paged and Posts. We can convert the post one to portfolio.

4. After we convert the post to portfolio, we'll likely get an error saying our `allWordpressWpPortfolio` is not defined. Thats because there is a const declaration up above the create pages section, which likely has something like `const { allWordpressPage, ..` and we need to make sure we've replace post with `allWordpressWpPortfolio` .

Granted this is an overview, not a step by step.

After all those things are plugged in and talking to each other, we can restart the Gatsby server and we _should_ be able to see our fancy new content type posts under whatever url we gave it. Likely something like `/posts/whatever`.


