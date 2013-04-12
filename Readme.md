Markable Remarkably Simple Blogging {{meta}}
--------------------------------------------

### Overview

This script accepts Markdown as input and builds a blog
style website.

### Quick start

You should download the source, place Markdown files in the posts
directory, and run build.

If you'd like to sort your posts, you need to have your naming format
be alphanumerically and lexicographically sortable. The naming standard
that's built into Markable is `[YEARMNDY]["Title"].md`.

If you'd like the date displayed in your post, you'll need to use something
like this:

    This is the title of my post {{meta}}
    -------------------------------------

The `{{meta}}` will be replaced by a date and a clickable link to a page
with only this post.

Replace the metadata in `build.pl` to get a custom title for your site.

The title and URL of every post in the browser is determined by the filename,
everything else in the file is determined by you.

To edit the About page, edit `about.md`.

### Design Goals

The design goals of this project are the same as the design goals of my website:

- Simple, easy, lightweight
- Scalable, fast web-hosting
- Custom domain name
- Cheap or free
- Write posts in Markdown alone

### Comparable Tools

I do not at all claim to have feature parity with these services,
but I looked into these static blog generators before deciding to 
write my own:

- [Ruhoh](http://ruhoh.com)
- [Jekyll](https://github.com/mojombo/jekyll)
- [Octopress](http://octopress.org)

### To do

- Categories
	- Each folder in the posts directory will be a category
	- Each category will have its own index
- Tags
	- A hashtag implementation *a la* Twitter
	- A hashtag in a post will enter that post into a
	  ordered list in a unified `Tags.html` page.