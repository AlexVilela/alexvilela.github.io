---
title: "How to build a static blog"
header:
  teaser: "/assets/images/posts/build-a-static-blog/blog-inner-peace.jpg"
tags:
  - static
  - simple
  - automation
---
When [I decided to start a blog]({% post_url 2019-02-09-why-I-started-a-blog %}) there were a few things that I quickly found out from other people that I admire.
### 1. Always own your data
When you use blog providers like Wordpress, Facebook, Disquss, etc, the data isn't owned or controlled by you. Moving away from these providers is often hard and you may not be able to move everything that you'd like.  

### 2. You may have to host your own blog
This was the hardest bit. I wanted to have a blog but didn't want to manage servers, deployments, connectivity issues, let alone pay for the hosting.

This tweet describes what I'd like to avoid:
<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">And seems like my blog is down due to connectivity issues with backend DB. Yay .NET and RavenDB.</p>&mdash; Itamar Syn-Hershko (@synhershko) <a href="https://twitter.com/synhershko/status/926001252466601984?ref_src=twsrc%5Etfw">November 2, 2017</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

Following up from that he suggests using a static website and this is what I'd like to cover today, how I this website works, currently completely static, including the comments.

### Extra requirements
Besides not wanting to manage servers, deployments and backups I also wanted the ability to control a little bit of the style and design without having to go too deep into HTML and CSS.

Markdown is a good solution for doing exactly that.

### Chosen Solution
In short, these are the solutions that I chose:
1. Static blog engine: [Jekyll](https://jekyllrb.com/). It supports Markdown and is simple enough to learn and use ([you can host it locally]({% post_url 2019-03-12-host-jekyll-locally %}))
1. Static comments: [Staticman](https://staticman.net/)
1. Hosting: [GitHub Pages](https://pages.github.com/) works well for me while also providing version control.
1. Blog theme: [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) is a great theme. Design and styling aren't my best strengths and this theme makes everything looks great with minimal effort.

<br>
The process that I follow is quite simple:
1. Write post locally
1. Look at how it looks like on a local Jekyll environment
1. Push to GitHub once I'm happy with it

And that is pretty much it. Behind the scenes GitHub pages will compile the source that I just pushed into a complete html static site and automatically deploy it to their production environment.

This is a good idea as I can focus on writing content without having to worry about hosting, backups, performance, scalability, etc. It brings me great peace of mind.

{% include figure image_path="/assets/images/posts/build-a-static-blog/blog-inner-peace.jpg" alt="Blog Inner Peace" caption="Blog Inner Peace (from https://www.illawarramercury.com.au/story/5230856/find-the-time-to-calm-your-mind/)" %}