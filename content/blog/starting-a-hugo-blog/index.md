---
title: "Starting a Hugo Blog"
date: 2022-11-14T14:07:10-07:00
summary: Checking out this blogging thing. I hear it's gonna be big.
draft: true
---

The death of the personal blog will always be a bummer to me. There was something nice about reading your friends or some other interesting person's thoughts on a webpage that took even a little bit of effort to create. Social networking websites seem to be having some tough times at the moment, but its easy to see why they captivated more people. It was easier to share your life with your friends when it was more bite-sized and photo/video-driven -- the phrase "micro-blogging" enters my head when I think about this shift in the early 2010s. But as the term "social networking" morphed into the nebulous phrase, "social media," we stopped sharing our lives with our friends and started horking down news videos and memes.

I'm not here to write a think piece about social networking in 2022. I'm not qualified to weigh in on that, even though I sort of did in the last paragraph. I'm here to talk about creating this blog with [Hugo](https://gohugo.io/)!

{{< youtube 0RKpf3rK57I >}}

I've spent a lot of time in the past working with HTML and CSS (mostly [Bootstrap](https://getbootstrap.com/)) to create simple, static pages that are easily hosted on a machine in my house or on Amazon S3. Working with those tools in the past was always something I enjoyed, but I have next to no desire to pretend to be a website designer again. Instead, I want to focus on the workflow and creation of blog posts. I noticed that my friend, [Geoff](https://pado.name/), had a simple and straight-forward website and blog, so I asked him what he used, and he turned me on to Hugo.

One of the key features of using Hugo to write blog posts that caught my attention was that I can write plain text [Markdown](https://daringfireball.net/projects/markdown/), and your template handles the rest. One of my previous personal websites was completely generated using [R Markdown](https://rmarkdown.rstudio.com/), and I loved that I could create webpages using the same markup language that I used to document code. While I don't write much R code anymore, one of the things that stuck with me was this idea of utilizing a website generator to create your static pages. This was important to me when writing papers when I was in grad school, but I always thought that it would be cool to create a personal blog that I could write with Markdown, so here we are.

The Hugo documentation pages are _mostly_ for folks who want to make their own themes and do minor web design using Golang templates, but so far I have been able to bob and weave past any of those grander objectives with regards to this website. For now, I'm a big fan of the [Blowfish](https://nunocoracao.github.io/blowfish/) theme, and I intend to use it for a long time.

As for deploying and hosting this website, I've decided to concede to the modern practice of using GitHub Pages and GitHub Actions. And you know what? It's really slick. Like, for real, I just added a standard-issue Hugo workflow yaml to the `.github/workflows/` directory of this website's [GitHub repository](https://github.com/zfleeman/zfleeman.com), and it rendered the static pages and hosted them using [GitHub Pages](https://pages.github.com/) within seconds. Good show! I'm sorry I ever doubted you, GitHub Pages. Granted, this is not as over-engineered as I like my projects, but using S3 and AWS CloudFront to host a website costs a _money_ (pennies, but still), and this is free! Right?