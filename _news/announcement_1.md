---
layout: post
title: Switching to al-foio jekyll theme
date: 2019-08-18
inline: false
---

I came across a new Jekyll theme on one of the NeurIPS conference pages and thought it would be perfect for my blog.
Here are some notes on how I switched to this theme.

***

* Fork repo <https://github.com/alshedivat/al-folio>
* Rename the cloned repo to `sanzgiri.github.io`

{% highlight bash %} 
git clone https://github.com/sanzgiri/sanzgiri.github.io
cd sanzgiri.github.io
bundle install
{% endhighlight %} 

* Make your changes.
 * Edit `_config.yml`
 * Edit `_pages/about.md`
 * Copy profile picture to `assets\img\prof_pic.jpg`
 * Generate bibtex for your publications from Google Scholar and paste in `_bibliography/papers.bib`
 * Remove content from `_data/coauthors.yml`
 * Edit news items (`announcement_N.md` files) in `_news`
 * In `_pages`, replace `teaching.md` with `classes.md`. Add any online MOOCs / Safari Training / LinkedIn Learning classes here.
 * In `_pages`, create `conferences.md` and list conferences attended.
 * Copy .md files for blog posts from older jekyll blog to `_posts` 
 * Add project files to `_projects` directory (not yet done)
 
* To deploy them and update your site: `./bin/deploy --user`

