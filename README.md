# Responsive email template

Greenpeace-themed **responsive** email templates for **quick** email **layouting**, **design** or development.

## About this templates
+ They use the [INK](http://zurb.com/ink/) framework, already tested with many mail clients
+ They use [Jekyll](http://jekyllrb.com/) and [Yaml](http://www.yaml.org/) to be easier and quicker to modify content
+ Jekyll url-encodes Twitter and other social networks links
+ Can be easily adapted to many mail sending services
+ It's easy to create AB tests with content, design or layout
+ Automatic Google Analytics campaign URLs

## Develop mails in Github.com or locally?

You can develop emails in Github or locally in your computer. 

### A - In Github.com
+ **Easily preview your emails.** - Github creates a webpage with your email if you develop it in the **gh-pages** branch. Your team can follow up your changes. Example: Committed changes to [this text](https://github.com/osvik/m-templates/blob/gh-pages/newsletter/index.html) will immediately change [this page](http://osvik.github.io/m-templates/newsletter/index.html). 
+ **No software to install** - All editing can be done online
+ **Accept collaboration** - With Github it's easy to fork, translate and improve content or design

_Instead of Github you can use Bitbucket's free private repositories to collaborate,  but instant previews will not work._


### B - Locally in your computer
+ **Privacy** - Emails and change history can't be read in the repository Github page
+ **Work offline** - layout emails without an Internet connection
+ Collaboration is not as easy as in Github
+ Users have to use very easy command line tools (Installing this tools may not be as easy for some users)


## In-linearize CSS
In emails CSS should go inline, as some mail clients do not interpret &lt;style&gt; tags. You should in-linearize your email's CSS before uploading to your mail software.

+ Online you can use the **[Inliner](http://zurb.com/ink/inliner.php)**
+ Locally you can use **[Premailer](https://github.com/osvik/m-templates#2---premailer)**

## Install software to layout emails without an Internet connection

If you need confidentiality in your email's content or your email development process you should not layout your emails in Github. Install the following software and do it locally:

### 1 - Jekyll

For some users may be as simple as typing:

`gem install jekyll`

in the terminal/shell.

[More info](http://jekyllrb.com/docs/installation/)

### 2 - Premailer

For some users may be as simple as typing:

`gem install premailer`

in the terminal/shell.

[More info](https://github.com/premailer/premailer)

### 3 - Git

It's also recommended, but not mandatory, that you [download and install git](http://git-scm.com/downloads/).

## Quick how to

### Generate html with Jeyll

In your terminal or shell:

`cd path/to/your/email/source/`

`jekyll build`

### In-linearize CSS with premailer

`cd path/to/your/email/output/`

`premailer index.html > linearized.html`

### Create A/B's

Use create git branches with A/B tests and merge the wining variants.
