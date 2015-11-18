---
post: true
layout: post
title:  "Open Graph"
date:   2015-11-17 10:30:59
categories: Open Graph
description: Meta-data for sharing on social networks.
blogimage: /images/post/og.png
ogimage: /images/og/logo200x200.png
image:
---
##
The Open Graph implementation was a bit of headache for me, probably mostly because I don't use Facebook that much and I have
never shared another website or article on Facebook or anywhere else so it took some time just understand what it was really for.
I spent a lot of time implementing og-tags only on my blog-post, then i realised that all the pages on the site should have og-tags,
they should only be typed different. I choose article for the blog posts and all the rest of the pages are typed as website.

The following code is written in a seperate HTML-file then included in all the files with the static site generator. It contains two if statements one is
which image to use when for example a blogg gets shared on Facebook, if there is a specific image use that else: use the standard logo.
The other if statement determines if a page is a post or just a part of the website and then sets the type accordingly.

{% highlight ruby %}


{% if page.image %}
<meta content="{{site.url}}{{ page.ogimage }}" property="og:image">
{% else %}
<meta content="{{site.url}}/images/logo200x200.png" property="og:image">
{% endif %}

{% if page.post %}
<meta content="article" property="og:type">
{% else %}
<meta content="website" property="og:type">
{% endif %}
<meta property="og:title" content="{% if page.title %}{{ page.title }}{% else %}{{ site.title }}{% endif %}">
<meta property="og:url" content="{{site.url}}{{page.url}}">
<meta property="og:description" content="{% if page.description %}{{ page.description | strip_html | strip_newlines | truncate: 160 }}{% endif %}">
<meta property="og:site_name" content="{{ site.title }}">

{% endhighlight %}

all of the information in the Open Graph data are generated automatically with the static site generator.
