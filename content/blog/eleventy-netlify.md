---
title: Hello World! - Eleventy + Netlify = Awesome
description: A foray into the Eleventy Static Site Generator
date: 2023-08-06
tags:
  - web dev
  - blogging
  - deployment
  - hosting
---

Once upon a time, I wanted to blog about interesting tech things.
I'd read enough on Hacker News about devs who spent too much time reinventing the wheel or [bikeshedding](https://www.techtarget.com/whatis/definition/Parkinsons-law-of-triviality-bikeshedding) when it came to building a blog, and I didn't want to fall into that trap.

"Should I just . . . Wordpress?" I wondered. I do love and respect what WP has done for making the web accessible to so many folk, but . . . it's also a bit of a dumpster fire.

And for a basic blog, I really don't need JS, or a database, or plugins. At the end of the day, what I needed was html, css, a few hosted images, and a way to deploy it all.

Enter: the Static Site Generator!

Generally speaking, a static site generator takes raw data, in my case, Markdown files, and spits out static html files.

### Advantages:
1. **Speed**: Since all pages are pre-built, they're blazingly fast to serve - it's like serving a pre-packaged sandwich, rather than cooking a full gourmet meal for every visitor! EthanStark.com is only 7.6KB and scores a 99/100 on Pingdom's [speed test](https://tools.pingdom.com/#62acc1645b800000). By comparison, my (admittedly not optimized) 2009 Wordpress [blog](https://sailingtrip2009.wordpress.com/) took 1.85 seconds to load its 1.3MB, scoring a [62/100](https://tools.pingdom.com/#62acc3ea0f000000).
1. **Security**: Without a server dynamically processing information and user requests, there are fewer opportunities for malicious activity.
1. **Version Control**: Everything lives in your codebase, making version control a breeze in comparison to the regular backups required by WordPress.
1. **Cost-Effective**: Hosting static files is generally less expensive and more straightforward than maintaining dynamic server resources. [Netlify](https://www.netlify.com/pricing/) will host your site for free, and even provide a free SSL certificate! (No referral links, I'm just a fan.)

### Cons of a Static Site Generator:
1. **Ease of use**: Static site generators are generally geared towards developers, and require some technical know-how to set up and maintain.
1. **Dynamic Content**: A SSG can't host your e-commerce site, or handle user logins, for example.

### Why Eleventy?
Eleventy is a JavaScript-based SSG. It's got great docs, a helpful community, and a nice [starter repo](https://github.com/11ty/eleventy-base-blog) that I based this site on.

### Deploying to Netlify
I make changes to my blog, build it locally, and push it to GitHub. Netlify automatically detects the changes, builds the site, and deploys it. It's lovely. 
