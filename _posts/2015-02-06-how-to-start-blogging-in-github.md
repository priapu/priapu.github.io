---
layout: post
title:  "How to start blogging in Github"
date:   2015-02-06 17:39:10
categories: jekyll github
---

Note: this is a TL:DR version.

* Install [Jekyll](http://jekyllrb.com/): `gem install jekyll`.
* Create an account at [Github](https://github.com/), and then:
** [Generate an `SSH key`](https://help.github.com/articles/generating-ssh-keys/) if you don’t have it already.
** Add the key to your [Github profile](https://github.com/settings/ssh).
* Read the manual at [Github pages](https://pages.github.com/). Basically it says:
** Create a new repo named `your_git_username.github.io`.
** Clone that repo: `$ git clone your_git_username.github.io`
** On the the project directory, initiate jekyll: `~/your_git_username.github.io $ jekyll new .`
** Start posting by putting Markdown formatted files inside `_posts` directory.
** Push your changes to the `master` branch and watch your blog go live.
* Profit!

Additional resources: 
* [Jekyll documentation](http://jekyllrb.com/docs/home/).
* [Jekyll themes](http://jekyllthemes.org/).
* [Markdown syntax documentation](http://daringfireball.net/projects/markdown/syntax).
* Syntax highlighting using [Pygments](http://pygments.org/).
