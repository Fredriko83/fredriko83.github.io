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
## Starting out with a template
I have not by any means created this site from scratch, I started out with a template from Jekyll and most of the time
I have put into this have been modifying code or picking through the code for snippets I can use elsewhere. Now when my
design is as finished as it's gonna get before I'm handing this site in to my teachers and I need to write this blog post to
describe how I used CSS preprocessor and static site generator (in this case Jekyll which includes Sass) it's really hard to
see how the things I have done to the Jekyll template could have taken almost 50 hours, It feels like I have only moved the
navigation out from the header, slapped som color on the page, implemented Open Graph and put a facebook share button on the page,
and put pictures with the posts on the front page. Since the deadline is creeping up on me I will just put the answers to the last
questions here:

##What do you think of pre-compiling your CSS?
I have really enjoyed working with both pro-compiling CSS and Static site generator. It's adds an extra layer of complexity and
when I didn't stick to using variables for colors it soon got confusing, should i change colors in the main.scss file or int the layout.
Sometimes i didn't remember which part of the site I had set to a color variable which resulted in several objects changing
color when i only wanted to change the color of a border. One problem with using a template is that I have ha to learn thier
way of structuring the CCS, maybe if I done it from scratch it would have ended up the same way but at least then i would
know where everything was, now a lot of time have been spent just figuring everything out. I think in the long-term pre-compiled css
will be a lot faster and easier than regular css but only as long as I work with it regular basis.

###Which techniques did you use?

More then the variables for colors it was mostly straight forward CSS.

### Pros & Cons

I think that the added complexity is a con and the way you can fast changes is a pro.

##What do you think of static site generators?

I really like it, when I realised that I could just add a .md file to the root and then a new page complete with link in
the navbar was generated, it was a little bit like magic :) Even though i haven't had time to do a lot of the things I would like do,
for example I wanted the posts to automatically get relevant images depending on their topics, I will have to fix that later when
I know what I will post about.

###What type of projects are they suitable for?
I think most sites online would be a good fit, as long as you are presenting something for example a company, personal sites & sites
containing information.
