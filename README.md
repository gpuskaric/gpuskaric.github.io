# [gregpuskaric.com](http://gregpuskaric.com/)

Greg's landing page and blog.

## Writing Posts

New posts go in the `_posts` directory.  To create a new post, create a new file in the `_posts` directory like this:

### Create a new file

To create a new file, navigate to the `_posts` directory and click on **Create new file** in GitHub.  

![adding a new file](images/create-file.png)

Name your file following this format:

```
YYYY-MM-DD-your-posts-name.md
```

![naming new file](images/naming-post.png)

After naming your file, you can either start editing it using [markdown](https://guides.github.com/features/mastering-markdown/) or you can click the green **Commit changes** button beneath the file editor to add the empty file.

### Front matter

All posts need to begin with some front matter, here's the default for this theme:

```
---
title: "Post Title"
categories:
  - post
  - general
tags:
  - example
  - formatting
---
```

For examples of what posts should or could look like, look at the [list of posts](https://github.com/mmistakes/jekyll-theme-unit-test/tree/master/_posts) used in this site [sample](https://github.com/mmistakes/so-simple-theme).

There's a ton of post types, [here's what these look like rendered](https://mmistakes.github.io/so-simple-theme/posts/) in a un-modified version of your theme - you should be able to map them back to the [sample post markdown](https://github.com/mmistakes/jekyll-theme-unit-test/tree/master/_posts).

### Writing Content

All content is written in **[markdown](https://guides.github.com/features/mastering-markdown/)** - a markup language that is like plain text but some html flair.

#### [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

If you need examples, look back at those sample [posts](https://github.com/mmistakes/jekyll-theme-unit-test/tree/master/_posts) or even look at this readme file directly in GitHub.  It should be self explanatory.

Use the **Preview** tab to see your changes when editing in GitHub.

## Editing Structure

The site is essentially a standard static site with HTML and CSS, except for that it uses a lot of templates to build stuff and pull things together.

Essentially what you need to know is that styles are in the `_scss` folder, html layouts are in the `_layouts` directory, and snippets/templates that get pulled into pages are in the `_includes` directory.

Things are named pretty obviously (like head.html is the head element of your site).

### Editing Locally

If you make changes on GitHub and commit to master your changes will be live immediately.  This is annoying when testing site structural changes.  It's possible to instead clone this repository and run it locally to test your changes.

At a high level (google 'cloning a repo')...

* open Terminal (mac) and `cd` into a directory you want
* run `git clone https://github.com/gpuskaric/gpuskaric.github.io.git`
* open the folder and make changes in whatever editor you want (I use [atom](https://atom.io/))

Then you have to make your changes, and to preview, you have to use [Jekyll](https://jekyllrb.com/)

To install Jekyll and preview...

* run `gem install jekyll bundler`
* in your project folder run `bundle exec jekyll serve`
* view your changes on your local host `http://127.0.0.1:4000/`

To push your changes live to the repo:

* in your project folder run 
  * `git add .`
  * `git commit -m "saving changes"`
  * `git push`
  
Troubleshooting this is as easy as googling first and texting me otherwise.

## Standard customizable files

* `_config.yml`
* `_navigation.yml`
* `_sass/so-simple/_variables.scss`

All images get added to `images/`
