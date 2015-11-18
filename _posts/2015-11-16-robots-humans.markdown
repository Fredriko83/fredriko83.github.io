---
post: true
layout: post
title:  "Robots & Humans"
description: humans.txt present the people behind the site.
date:   2015-11-16 15:14:29
categories: Webdevelopment
ogimage: /images/og/logo200x200.png
blogimage: /images/post/robothuman.png
image:
---
The robots.txt and humans.txt are both text files that can be found in the root of a website.


### robots.txt
The robots.txt contains information for crawlers, for example google, and lets the crawlers know which (if any) parts of the
site that should be indexed. In my case even though my page site is as finished as its gonna be right now I don't fell ready
to set it free. That's why my robots.txt (can be found here [{{site.url}}/robots.txt](/robots.txt)). contains the following:

{% highlight ruby %}
User-agent: *
Disallow: /
{% endhighlight %}

The first line means all crawlers/robots and the second line means that they are not allowed to index this site. To open the site up
and make it possible for all crawlers to index it we can just remove the "/" like this:

{% highlight ruby %}
User-agent: *
Disallow:
{% endhighlight %}

And if we where to only let Google index the site we would do it like this:

{% highlight ruby %}
User-agent: Google
Disallow:

User-agent: *
Disallow: /
{% endhighlight %}

robots.txt is not in anyway a security measure, the only thing the robots.txt does is telling the robots if and by what robots
it want to get indexed but if a robot for some reason want to index the site anyway there is nothing in robots.txt that can stop it.

There is more information about robots.txt at [http://www.robotstxt.org](http://www.robotstxt.org)


### humans.txt
The humans.txt is a way for people that have taken part in the creation of the website to show it. Often the owner of the site
doesn't want the creator to clutter the site with information about who made it and then you can put that in humans.txt instead.
The file which only sits in the root of the website have no impact on the website and can be accessed by adding humans.txt to the url, for
example if you would like to see this sites humans.txt you would have to go to
[{{site.url}}/humans.txt](/humans.txt).

{% highlight ruby %}
/* TEAM */

All in all: Fredrik Olsson.

Twitter: {{ site.twitter_username }}.

Location: Broby, Sweden.

/* SITE */

Last update: {{ site.time | date_to_rfc822 }}.

Standards: HTML5, CSS3,..

Software: Webstorm, Photoshop.
{% endhighlight %}

You can read more about it over at [http://humanstxt.org](http://humanstxt.org).

