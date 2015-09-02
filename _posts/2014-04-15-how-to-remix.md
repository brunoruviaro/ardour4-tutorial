---
layout: post
title: "How to Remix"
description:
comments: false
tags: [07 APPENDICES]
image:
  feature: Ardour3_Empty_Session_Transparent.png
  credit:  
  creditlink:  
---

Thanks for your interest in remixing this tutorial.

You can rewrite, add, delete, reorder, basically do whatever you want to the tutorial, and have it automatically published on your GitHub account.

Basically, you just need to follow the same steps described [here](../how-to-contribute-3), but instead of creating pull requests to merge your changes into the original tutorial, you simply let your tutorial exist by itself, and use your own link to distribute it (on the GitHub online interface, click "Settings" from your repository page, and you will find the link it's being published to).

Here's some additional information on how to customize the tutorial to look like the way you want:

### Change main title of tutorial

This is done inside *_config.yml*. There you can change title, description, estimated reading time, etc. It's the same file where you change the url (localhost or online website).

The fields "owner name, avatar, bio" in that file define the text and image to be displayed in the "about" pop-up box.

#### About the \_config.yml file

Note that *_config.yml* is in the .gitignore file. This allows you to work locally (with your config file pointing to localhost:4000, but avoid having that change be uploaded to the main online repository). In your online repository, you do want to have the url to point to the actual url of your tutorial. Easiest way is probably to just do a one-time edit of *_config.yml* directly on GitHub website (put your new title, proper url, etc). Then commit, and clone your repository after that. Make the change to localhost:4000 locally, and work from there.

### Change background picture

This is done in the file *ardour4-tutorial/index.html*. The current default image is *Ardour3_Empty_Session_Transparent.png*. Replace it with any other file that you have saved inside the **images** folder.

To change the background picture of individual posts, open the post file itself (extension .md) and change picture file name in the header.

### Change subtitle under main title

Also inside *index.html* you can change the subtitle "BEGINNER'S TUTORIAL" that shows up in the main page (it's the line "title" right below layout: post-index)

You can now go ahead and remix the tutorial in any way you like.

### Further Help with GitHub

Simple git guide for beginners:
[http://rogerdudler.github.io/git-guide/](http://rogerdudler.github.io/git-guide/)













**Appendices:**
[FURTHER HELP](../further-help)   ||
[GLOSSARY](../glossary)   ||
[LINKS](../links)   ||
[CREDITS](../credits)
