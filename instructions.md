---
layout: page
title: "Instructions for Alyssa"
subtitle: "step by step"
permalink: /instructions/
---


# What I need from you:

### Text:

- Title you want on the page tab
- <del>About me section</del>


### Images:

- main image for homepage and about section (can be different)
- Images for gallery. Each image will need:
    - jpg or png file, somewhere around 1000x700px to 1920x1080px in size
    - another thumbnail file, 150px in height
    - title
    - any other information you want to see in a caption
    - a date
    - an order number if you care about that
- square image for the tiny logo on the tab. Give me a small square image no smaller than 310x310px.

### Links:

- any social networks you want to link to? I already included twitter and fb (see the logos in the top right)
- I was thinking maybe we can link to past or upcoming shows on the about or contact page too, what do you think?


### Changes:

- let me know any aesthetic changes you want to colours, placement, fonts, etc
- any bugs you see
- also etransfer me $14.12 for the domain when you get a chance. (The email receipt i sent was in USD)


# How to setup your computer

Take a deep breath and get ready to learn some stuffs.

## Terminology to know

#### Git:

A convenient way to manage changes to code and content. Any changes you make are easily reversible and previous content is never lost if you make a mistake.

#### Github:

Basically a cloud storage version of git so we can collaborate, publish the site, and nothing gets lost.

I have made you a [github](http://github.com) account:

user: alyssaschroder
pass: jessjess123

You will need this account to make changes to the site.

#### Terminal:

Allows you to type commands that directly speak to the computer. I have provided you some basic commands to run in order to save and publish your changes, but more on that later. You can also run them by double clicking, but this way you can feel like a hacker. ;)

#### Markdown:

Markdown is a markup language. It allows you to write readable html content without any knowledge of html. The content on your pages is all written in markdown, and then converted into html after it is published. (You can of course write it in html instead if you like.)

For example to _italicize_, write `_italicize_`, or **bold** write `**bold**`.

Full rundown of the syntax [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

## Steps to follow to setup your environment:

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
- install git gui for later

# Making changes

Follow these steps to make any changes.

1) **Start**: Paste the following into the terminal and press enter (i.e. run these commands):

    cd ~/alyssa-portfolio;
    ./start;

This step ensures any changes I have made are now downloaded to your computer.
Don't worry too much about the output from this.

2) Make any changes, and preview them as necessary (more details on this to follow). When you are satisfied with your changes, continue to the next step.

3) **Save**: Run the following:

    ./save "my save message here"

Be sure to include a save message (in quotes) that summarizes what you added!
This command will take any changes you have made, and save them on github as a backup, as well as allowing me to see any changes you've made.
**This does not publish to your site!** Use the `./save` command **before** publishing, or if you want to save progress without seeing your changes live.

4) **Publish**: Run the following:

    ./publish

This command publishes any changes you have saved to alyssaschroder.com.
This is always reversible, but it is best to preview your work prior to publishing it.
After running the `./publish` command you should see your changes live within a few minutes.

And thats it! If at any point you get stuck, something doesn't work, or you get an error message, just copy paste the output from the commands to me.


## The code: which files should you care about?
Open finder and look at the `alyssa-portfolio` directory under your home directory (likely called `alyssaschroder`). Here you will see a whole bunch of folders and files that you don't need to care about. The only ones you need are as follows:

- **instructions.md** -- contains this information.

- **about.md** -- contains the content for your about page. If you ever want to change the text or images on that page, look here.

- **index.html** -- this is your home page. Edit this if you want to change the content there.

- **contact.md** -- content for contact page.

- **/_posts/** -- this directory contains data for the images in your galleries. See "Adding a new image" below for more details on these files.


##Adding a new image

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


## Previewing changes

In order to preview your changes, open a terminal and run the following:

    cd ~/alyssa-portfolio;
    jekyll serve --watch;

You should now see your local files at `localhost:4000` (type this into the address bar in your web browser).


# Want to learn more!?

If you want any explanations of computer speak, just let me know. :P
If you prefer to pick and choose which files to publish or save as backup, there is another way I could show you after you're comfortable with the tools I have given you.
