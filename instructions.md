---
layout: page
title: "Instructions for Alyssa"
subtitle: "step by step"
permalink: /instructions/
---

#What I need from you:

####Text:
- Title you want on the page tab
- ~~About me section~~


####Images:
- main image for homepage and about section (can be different)
- Images for gallery. Each image will need:
    - jpg or png file
    - title
    - any other information you want to see in a caption
    - a date
    - an order number if you care about that

####Links:
- any social networks you want to link to? I already included twitter and fb (see the logos in the top right)
- I was thinking maybe we can link to past or upcoming shows on the about or contact page too, what do you think?


####Changes:
- let me know any aesthetic changes you want to colours, placement, fonts, etc
- any bugs you see


#How to setup your computer

Take a deep breath and get ready to learn some stuffs.

##Terminology to know

####Git:
A convenient way to manage changes to code and content. Any changes you make are easily reversible and previous content is never lost if you make a mistake.

####Github:
Basically a cloud storage version of git so we can collaborate, publish the site, and nothing gets lost.

I have made you a [github](http://github.com) account:

user: alyssaschroder
pass: jessjess123

You will need this account to make changes to the site.

####Terminal:
Allows you to type commands that directly speak to the computer. I have provided you some basic commands to run in order to save and publish your changes, but more on that later. You can also run them by double clicking, but this way you can feel like a hacker. ;)

####Markdown:
Markdown is a markup language. It allows you to write readable html content without any knowledge of html. The content on your pages is all written in markdown, and then converted into html after it is published. (You can of course write it in html if you want instead if you like.)

For example to _italicize_, write `_italicize_`, etc.

Full rundown [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

##Steps to follow to setup your environment:
1) Enable remote login on your computer, by following the steps [here](https://support.apple.com/kb/PH18726?locale=en_US).

2) go [here](http://git-scm.com/downloads) and click download for Mac. Run the install wizard and follow the steps.

3) (optional) go [here](https://www.sublimetext.com/3) to download sublime text 3 (a great text editor) You can also use TextEdit.app but I've never used this. For your purposes, either should be fine.

4) At this point I will remotely login to your machine and set some things up for you to download the code for you, allow you to preview changes before publishing, and allow you to publish changes. If you're interested... look [here](https://help.github.com/articles/generating-an-ssh-key/) for the complicated stuff.

5) Disable remote login on your computer (same setting as the first step) [here](https://support.apple.com/kb/PH18726?locale=en_US)

After these steps, you should be able to make changes and publish them!

Notes for Jess:
- Check git version to verify install.
- setup ssh key
- clone repo
- install ruby and jekyll so she can run a local server & verify


## Making changes

### The code
Open finder and look at the `alyssa-portfolio` directory under your home directory (likely called `alyssaschroder`). Here you will see a whole bunch of folders and files that you don't need to care about. The only ones you need are as follows:

- **instructions.md** -- contains this information. (so does README.md)

- **about.md** -- contains the content for your about page. If you ever want to change the text or images on that page, look here.

- **index.html** -- this is your home page. Edit this if you want to change the content there.

- **contact.md** -- content for contact page.

- **/_posts/** -- this directory contains data for the images in your galleries. See "Adding a new image" below for more details on these files.

### Adding a new image

Create a  new file in the `/posts/` directory. The file extension must be `.md` or `.markdown`. Alphabetical order dictates the order of the images in the galleries (if this is annoying for you, I can add change this).

The content of the file must follow this convention:

    ---
    layout: post
    title:  "YOUR IMAGE TITLE"
    image: "/images/filename.jpg"
    date:   2015-09-06
    categories: [sketches, watercolour-ink, acrylic]
    ---
     Caption goes here


Choose one or multiple categories your image belongs in.


### Previewing changes

TODO run jekyll serve --watch and go to localhost:4000 in browser

### Saving and Publishing changes

TODO

before doing anything run ./start

to save your changes, run ./save

publish run ./publish
