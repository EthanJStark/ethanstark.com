---
title: Hello World! - Building a Blog with Eleventy
description: Eleventy + Netlify = Awesome 🚀
date: 2023-08-06
tags:
  - web dev
  - blogging
  - deployment
  - hosting
  - ChatGPT
---

Once upon a time, I wanted to blog about interesting tech things.
Reading Hacker News, I was familiar with the trap many developers fall into - either reinventing the wheel or [bikeshedding](https://www.techtarget.com/whatis/definition/Parkinsons-law-of-triviality-bikeshedding) when it came to building a blog, and I didn't want to do the same.

"Should I just . . . Wordpress?" I wondered. I do love and respect what WP has done for making the web accessible to so many folk, but . . . it's also a bit of a dumpster fire.

For a minimalist blog, I didn't require the complexities of JavaScript, a database, or myriad plugins. My requirements were simple: HTML, CSS, some hosted images, and a hassle-free deployment mechanism.

That led me to discover the magic of **Static Site Generators (SSGs).**

In essence, an SSG transforms raw data (like my Markdown files) into static HTML files.

### Advantages:
1. **Speed**: Pre-built pages are incredibly swift to serve. For instance, this site, at a mere 7.6KB, boasts a a 99/100 on Pingdom's [speed test](https://tools.pingdom.com/#62acc1645b800000). In contrast, my 2009 Wordpress [blog](https://sailingtrip2009.wordpress.com/), which wasn't particularly optimized, clocked a loading time of 1.85 seconds for its 1.3MB took 1.85 seconds to load its 1.3MB, scoring a [62/100](https://tools.pingdom.com/#62acc3ea0f000000). Oh look, a [helpful graph](/blog/hello-world-11ty/eleventy-netlify/#wordpress-vs-ssg-a-helpful-graph)! 😉 
1. **Security**: Without a server dynamically processing information and user requests, there is a much smaller surface area for malicious activity.
1. **Version Control**: The entire content resides within your codebase, simplifying version control. This streamlined approach contrasts sharply with the periodic backups Wordpress demands.
1. **Cost-Effective**: Static files are typically cheaper and simpler to host, as opposed to managing dynamic server resources. Companies like [Netlify](https://www.netlify.com/pricing/) even offer free hosting and complimentary SSL certificates. (I must clarify, this isn't a sponsored mention. I'm genuinely impressed with their service.) 

### Cons of a Static Site Generator:
1. **Ease of use**: SSGs are primarily developer-oriented and demand a certain degree of technical expertise for setup and maintenance.
1. **Dynamic Content**: SSGs aren't the go-to solution if, for example, you're looking to host an e-commerce platform or manage user logins.

### Why Did I Choose Eleventy?
Eleventy is an SSG built on JavaScript. It stands out due to its comprehensive documentation, supportive community, and an excellent [starter blog repo](https://github.com/11ty/eleventy-base-blog) that was the foundation for this site.

The code for this site, which used that starter blog for its template, can be viewed [here](https://github.com/EthanJStark/ethanstark.com).

### Deploying to Netlify
I make changes to my blog, and push it to GitHub. Netlify seamlessly detects these modifications, builds the site using 11ty, and deploys it. The entire process is remarkably smooth.

### Wordpress vs. SSG: A Helpful Graph
"Hey, GPT-4 (Advanced Data Analysis Mode)--please generate a graph to represent the following:"

```text
"My Wordpress Blog": load time=1.85s. page size=1.3MB
"EthanStark.com - 11ty": load time=138 ms. page size=7.6 KB
```
{% image "./WP-vs-11ty.png", "Bar graph depicting the following: 'My Wordpress Blog': load time=1.85s. page size=1.3MB 'EthanStark.com - 11ty': load time=138 ms. page size=7.6 KB" %}

😎 Cool. Good job, robot.
