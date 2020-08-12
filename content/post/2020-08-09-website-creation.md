---
title: How I created this website
date: 2020-08-09
tags: ["webpage"]
---

This is my first post. I will record how I built up this website.
My ultimate goal is a website combining self-promotion and blog posting.
After cruising a lot online, I finally pinned it down to use *Hugo + GitLab*.
The factors I considered during this process include:

- Simple to maintain the website
- User friendly to write blogs
- Able to add tags
- Neat and clean design

Their importance for me decreases from top to down.
Balancing them, the current solution seems the best.

At first, I referred to the personal website of my two friends who are also pursuing their PhD degree. One is [Zhiyuan Yao](https://zyao.org/) and the other is [Junheng Hao](https://www.haojunheng.com/). The former is basically a technical blog, whose most modules are around blogging and even the 'Categories' and 'Tags' are redundant to appear on the menu simultaneously. The 'About' section displays some key personal information and research experiences. The latter is a standard academic website, which is organized from biography, publications and conference/workshop posters et al. I prefer the former one but want more places to demonstrate my research projects. Modifying based on it is a good try.

To build a webpage, you need a static site generator and a deployment server.

1. First try (Jekyll + GitHub Pages)

A good guide about this combination can be seen [here](http://jmcglone.com/guides/github-pages/). Because I am not a command line user, I tried my best to avoid using command lines. And I glanced at the local configurations of Jekyll, which is quite a pain in the ass for me. So I found a template free of any local configurations, [Jekyll Now](https://github.com/barryclark/jekyll-now). As it claimed, I set up a minimal blog in a few minutes. Then I found its shortcomings. I cannot add tags to posts and to be honest its layout is outdated. There are in fact lots of elegant themes for Jekyll, for example, the one used by [Zhiyuan Yao](https://github.com/simpleyyt/jekyll-theme-next). If you are a more hardcore coder and don't bother to set up Jekyll on your computer, it is much fun to play with it.

2. Second try (Academic + GitHub + Netlify)

Scrolling down [Junheng Hao](https://www.haojunheng.com/), I found two useful links. The first is [Academic theme](https://sourcethemes.com/academic/). This is a website builder framework using the [Hugo](https://gohugo.io/) static site generator as the core. If I understand correctly, it only uses GitHub repository to host the content as a local drive and achieves functions like version control. It is [Netlify](https://www.netlify.com/) but not GitHub that actually deploys the website. I tried to follow its guide and gave up halfway because to integrate three things seems too much for me (Yes, I am a lazy person).

3. Third try (Hugo + GitLab)

Finally, I shifted to [Hugo](https://gohugo.io/). Following its [Quick Start](https://gohugo.io/getting-started/quick-start/), I easily created a new site running on the local server. Hugo was installed using [Homebrew](https://brew.sh/) on my MacBook and more detailed video tutorials can be seen on the [YouTube](https://www.youtube.com/watch?list=PLLAZ4kZ9dFpOnyRlyS-liKL5ReHDcj4G3&v=qtIqKaDlqXo). Because Hugo renders static websites, I need to host my site virtually so that anyone on the Internet can access it. Hugo suggests a few popular hosting and automated deployment [solutions](https://gohugo.io/hosting-and-deployment/), including aforementioned Netlify and GitHub. But I was attracted by GitLab.

> > GitLab makes it incredibly easy to build, deploy, and host your Hugo website via their free GitLab Pages service, which provides native support for Hugo.

It turned out to be incredibly easy indeed. Then I found an even easier solution -- directly forking [the Hugo project on GitLab](https://gitlab.com/pages/hugo). You need to cross-refer to it and [GitLab Pages](https://about.gitlab.com/stages-devops-lifecycle/pages/). Eventually you will get a personal website meeting the above four requirements.

Several useful tools:
- Design icons and avatars using [Over](https://www.madewithover.com/)
- Maintain your local project by git GUI client for Gitlab using [GitKraken](https://www.gitkraken.com/) or [GitHub Desktop](https://itnext.io/how-to-use-github-desktop-with-gitlab-cd4d2de3d104) (If you are a user of both GitHub and GitLab, I recommend the latter)
- Edit your Markdown posts using [Atom](https://atom.io/) (I installed it a long time ago since I did not like the built-in text editor of macOS. I had never thought it could be so handy until I wrote this post. I highly recommend it to you) or [Typora](https://typora.io/)

As you can see, my problem solving is not linear but rather I tried different routes. I tend to adjust my current plan by dynamically reevaluating the effort investment in the near future as well as the long run usage cost. If it is not efficient, I will decisively give up the current route and try the next one until my goal is reached. But you should always stick to your final goal.

Hope this post will be helpful for you~
ヽ(✿ﾟ▽ﾟ)ノ

If you have any question, feel free to contact me via channels listed at the bottom of this page. I recommend reading a very useful article before formulating your question.

- [How To Ask Questions The Smart Way](http://www.catb.org/~esr/faqs/smart-questions.html)
- [提问的智慧](https://lug.ustc.edu.cn/wiki/doc/smart-questions/#%E5%8E%9F%E6%96%87%E7%89%88%E6%9C%AC%E5%8E%86%E5%8F%B2)
