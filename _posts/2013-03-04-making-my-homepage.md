---
layout: post
published: true
title: Making My Homepage with Jekyll and Bootstrap
category: Blog
tags:
  - Homepage
  - Jekyll
  - Bootstrap
---

Hello and welcome to my homepage! As the first real post, I figure that it would be appropriate to go over how this webpage was made (not that it is finished being made). The source is available through GitHub at <https://github.com/te0d/te0d.github.com>.

My initial intention of registering the domain `http://todonnell.us` was to use it solely as a place for my resume and portfolio. Instead, I decided that I should also maintain a blog chronicling my various projects. In the past I have mainly used Wordpress as blogging software. This time I decided to use [Jekyll](https://github.com/mojombo/jekyll) - a blog-aware, static site generator written in Ruby. This decision was made easier since I am hosting it through [GitHub Pages](http://pages.github.com/) which can generate the site using Jekyll directly from my page's GitHub repository.

Jekyll
------

Since Jekyll generates a static site, there is no need for server-side scripting to change the content of the pages making it usable on nearly any web server. What Jekyll provides is the ability to reuse segments of HTML as well as utilize other markup languages. The layout of a Jekyll site is as follows ([explained in more detail on the wiki](https://github.com/mojombo/jekyll/wiki/usage)):

        .
        |-- _config.yml
        |-- _includes
        |-- _layouts
        |   |-- default.html
        |   `-- post.html
        |-- _posts
        |   |-- 2007-10-29-why-every-programmer-should-play-nethack.textile
        |   `-- 2009-04-26-barcamp-boston-4-roundup.textile
        |-- _site
        `-- index.html

The directories and files which begin with an underscore are special folders used by Jekyll to generate the static pages. Files in the root directory can use [YAML Front Matter](https://github.com/mojombo/jekyll/wiki/yaml-front-matter) to use layouts in `_layouts` and include segments of HTML from `_includes`. YAML Front Matter provides a way to use "variables" (a way to pass metadata between pages) in the generation of static pages. The `_posts` directory is used to contain blog posts. The post file names need to include the date as shown in the layout so they can be organized by date in the generated directory.

Bootstrap
---------

[Bootstrap](http://twitter.github.com/bootstrap/)([GitHub repository](https://github.com/twitter/bootstrap)) is a framework made by Twitter used to make designing web pages easier. More specifically, Bootstrap is good at making web pages with a modern design and display well across a [variety of devices](http://twitter.github.com/bootstrap/scaffolding.html#responsive). The modern feel is acheived with Bootstrap's [CSS for fundamental HTML elements](http://twitter.github.com/bootstrap/base-css.html). Another useful feature is the [grid layout](http://twitter.github.com/bootstrap/scaffolding.html#gridSystem) it provides which only requires setting the appropriate `<div>` class attributes to position the `<div>`.

My webpage does not venture far from [the examples](http://twitter.github.com/bootstrap/getting-started.html#examples) yet, but it is recommended to customize the design with your own CSS.

