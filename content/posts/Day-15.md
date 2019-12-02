---
title: Day 15
date: "2019-10-27"
template: "post"
draft: false
slug: "/posts/day-15/"
category: "100 Days of Code"
tags:
  - "Web Development"
  - "100daysofcode"
  - "Gatsby"
description: "Building a page with GraphyQL query."
socialImage: ""
---

 <h2>Building a page with GraphyQL query</h2>
<p>Okay wow, so as a front-ender this is a bit unsual for me.</p>
<p>Today we <Link to="my-files">build a page</Link> that uses the query we were just playing around with. Or really, a similar query that actually shows something worth showing.</p>
<p>Per usual, we start with a new page, import all the things at the top. Then we get to do one of my forced favorite things. Console log!</p>
  

![example code with console.log](../../static/media/Screenshot&#32;from&#32;2019-10-30&#32;05-44-54.png)

<p>Then we need to actually plop that query into our page. Remember folks, backtick with care `</p>
  

![showing graphiql query side by side with query in gatsby](../../static/media/Screenshot&#32;from&#32;2019-10-30&#32;05-48-32.png)

<p>We can nearly copy paste the query over from our GraphiQL explorer into our new page. In this instance we need to simplify it by dropping the "MyQuery" part. I bet having that exter name will come in handy in the future with multiple queries on a page.</p>
<p>Now that we've typed that all in, save that sucker and check your terminal. If you are like me, go ahead and fix all the typos, then go check your browser console.</p>
  

![browser console log of query](../../static/media/Screenshot&#32;from&#32;2019-10-30&#32;05-53-16.png)

<p>Yay, now we know we didn't mess it up. Now that we have the data and know it, we an display it. Continuing to follow along, we build out a table, and then we get to the nitty gritty of accessing said data</p>
<p>Again as a basic front-ender I'm not currently 100% on what we're doing here.</p>
  

![data access code](../../static/media/Screenshot&#32;from&#32;2019-10-30&#32;05-57-23.png)


<p>But it does give us the values we want to print out, and in my experience if its valuable we will likey be doing it agian. And again. Eventually it should sink in.</p>
  

![rendered data in the browser](../../static/media/Screenshot&#32;from&#32;2019-10-30&#32;05-59-49.png)

<p>Tada! we now have a table showing some stuff that we queried. <Link to="my-files">The page</Link>.</p>

<p>I'm sure you've noticed a difference in my returned data vs what is shown just in the example just above this <a href="https://www.gatsbyjs.org/tutorial/part-five/#whats-coming-next">link</a></p>
<p>My theory is they changed the code snippet in relation to the screen shot. It could also be that this current site isn't a 1 to 1 representation of the example gatsby site in the tutorial. It is likely a mixture of the two, leaning heavily on me not doing it right.</p>
<p>The important part though is that we have made our own query, returned it in a new page and displayed it with markup.</p>