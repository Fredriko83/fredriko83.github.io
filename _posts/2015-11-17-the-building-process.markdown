---
post: true
layout: post
title:  "Jekyll - The building process"
date:   2015-11-18 00:12:41
categories: Jekyll
description: How i went about building this site in Jekyll
blogimage: /images/post/jekyll.png
ogimage: /images/og/logo200x200.png
image:
---
## Starting ou with a template
I have not by any means created this site from scratch, I started out with a template from Jekyll and most of the time
I have put into this have been modifying code or picking through the code for snippets I can use elsewhere. Now when my
design is as finished as it's gonna get before I'm handing this site in to my teachers and I need to write this blog post to
describe how I used CSS preprocessor and static site generator (in this case Jekyll which includes Sass) it's really hard to
see how the things I have done to the Jekyll template could have taken almost 50 hours, It feels like I have moced the
navigation out from the header, slapped som color on the page, implemented Open Graph and put a facebook share button on the page,
and put pictures with the posts on the front page. Here comes in short what I have done, it doesn't look like much but it's been
damn hard!

### Moving <nav>
For some reason the first thing I did was to move <nav> from within the header.html to it's own file. There wasn't really a
point to this at least nothing I can remember now. But the way the site is designed now with a clear visual seperation between
the header and navigation field i guess it's good from a development standpoint -> It's easier to find find the code your looking for,
and it is easier to get a got overview over both header.html and nav.html when they aren't entangled.

### Implementing Open Graph.
I have already described Open Graph and how it was inplemented in a [previous post]({{site.url}}/jekyll/2015/11/17/open-graph.html)
