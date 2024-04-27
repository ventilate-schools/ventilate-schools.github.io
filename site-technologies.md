---
layout: page
title: Site Technologies
permalink: /site-technologies/
---

# Rationale for GitHub Pages and Jekyll

* GitHub Pages (GHP) is free for this use. Jekyll is a mainstream site-generation tech. This combo gives multi-year stability even without an admin team. All work could stop for a year and the site remains up - That's not true of dedicated Wordpress instances, and one one Wordpress.com would have a months fee.
* Git gives first class history to allow undoing of changes, or tracking bad actions back to an account.
* There are 1,460 schools in Wales. The rate at which schools are created, removed or renamed is slow enough for Git to be a fine choice versus a real database. This is "very small data" and after an initial flurry, changes to a page for a school would slow up.
* Lastly, changes can be made to 1480 school entries in bulk (batch) if needed (command line git checkouts), and still be in the history or audit trail.

Sure, contributing changes is harder for people without Git skills, but evey year 
more and more high/secondary school kids are being education on Git in particular
and version-control in general. GitHub itself has in excess of 100 million users
worldwide. The think that the skills needed for editing of pages within this site 
are teachable to people who've never used the tools before and through the web-UI.  
All your great grand-children will know how to use Git, or whatever replaces it.

# Rationale for Markdown language for page source

* It is ubiquitous these days for this particular use (Jekyll and other static-site-generators; SSGs)
* Hyperlinks, bolding are easy things to lean on top of it's "plain text" nature. Other people's primer: [https://www.google.com/search?q=leaning+markdown](https://www.google.com/search?q=leaning+markdown)

TODO: link to primer for our purposes