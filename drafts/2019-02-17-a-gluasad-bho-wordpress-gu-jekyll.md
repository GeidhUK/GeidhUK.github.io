---
title: A' gluasad bho Wordpress gu Jekyll
author: Crìstean MacMhìcheil
type: post
date: 2019-02-17 18:00:00
image: https://raw.githubusercontent.com/MacMhicheil/GeidhUK/master/images/2019-02-17-a-gluasad-bho-wordpress-gu-jekyll.jpg
categories: blog
tags: blog, GeidhUK, Naidheachdan Pinc, LCDTQ, Naidheachdan, ùrachadh, Jekyll, Wordpress
---

Until now Geidh.uk has been a self-hosted Wordpress blog running a custom theme and several third-party plugins. While it has served its purpose well, I was getting increasingly frustrated by slow page loads, server errors, downtime, constant updates and security risks, so as of today the site has moved from Wordpress to Jekyll.

<!--more-->

I've done my best to minimise the impact of the migration - old URLs should still work and the layout of the site is almost identical. However, please let me know on Twitter if you find something that doesn't work as expected.

The Tachartasan section of the old site relied on a third party Wordpress plugin which allowed to me enter the event information and it generated the calendar, event page, maps etc automatically. Unfortunately, I haven't come across

#### Dè th' ann an Jekyll?

Jekyll is a blog-aware static site generator (SSG) that takes a bunch of raw text files (including markdown files for the content) and spits out a bunch of HTML and CSS that you upload to your server. Instead of doing a whole bunch of database requests whenever you load a page, all of the hard work occurs when the site is generated - so the end user just loads some HTML and images stored on your server. This makes your site incredibly fast and lightweight, at the cost of losing access to “most” interactive features.

#### Buannachdan

* Free hosting on GitHub Pages
* Page loading time on the desktop is dramatically faster, and it’s probably even more noticeable on mobile.
* As your site content is all text files, you can get great version control with Git.
* The resulting site can be hosted practically anywhere - it’s just HTML, CSS and content files.
* It’s much easier to edit HTML/CSS to customise pages on your blog.
* No need for server backups: Assuming your site source is in Git and/or Dropbox, you can regenerate the site whenever you need.
* You can build your site offline, edit it and test it and choose when you upload (which requires having 2 versions of your site with WordPress).

#### Eas-bhuannachdan

* There isn’t always a nice alternative to your WordPress plugins.

#### Co-dhùnadh

Overall, I’m pretty happy with the migration to Jekyll and I feel it will be less of an effort to maintain. It’s been really nice to be able to get my hands dirty and edit CSS and page layouts for certain pages without hacking through WordPress template code and equally to be able to write the content in simple text files.

If you don’t need any super fancy features and find a good template that you’re happy with (or you’re happy to get your hands dirty) - I can recommend moving to Jekyll.
