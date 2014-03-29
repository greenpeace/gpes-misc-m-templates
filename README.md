# Responsive email template

Greenpeace-themed **responsive** email templates for **quick** email **layouting**, **design** or development.

## About this templates
+ They use the [INK](http://zurb.com/ink/) framwework, already tested with many mail clients
+ They use [Jekyll](http://jekyllrb.com/) and [Yaml](http://www.yaml.org/) to be easier and quicker to modify content
+ Jekyll url-encodes Twitter and other social networks links
+ Can be easily adapted to many mail sending services
+ It's easy to create AB tests with content, design or layout

## Develop mails in Github.com or locally?

You can develop emails in Github or locally in your computer.

### A - In Github.com
+ **Easily preview your emails.** - Github creates a webpage with your email if you develop it in the **gh-pages** branch. Your team can follow up your changes.
+ **Accept collaboration** - With Github it's easy to fork, translate and improve content or design
+ **No software to install** - All editing can be done online

### B - Locally in your computer
+ **Privacy** - Emails can't be read before they're sent
+ **Work offline** - layout emails without an Internet connection
+ Collaboration is not as easy as in Github
+ Users have to use very easy command line tools (Installing this tools may not be as easy for some users)

## In-linearize CSS
In emails CSS should go inline, as some mail clients do not interpret &lt;style&gt; tags. You should in-linearize your email's CSS before uploading to your mail software.

+ Online you can use the **[Inliner](http://zurb.com/ink/inliner.php)**
+ Locally you can use **Premailer**

## Install software to layout emails without an Internet connection

If you need confidentiality in your email's content or your email development process you should not layout your emails in Github. Install the following software and do it locally:

### 1 - Jekyll

For some users may be as simple as typing:

`gem install jekyll`

in the terminall/shell.

[More info](http://jekyllrb.com/docs/installation/)

### 2 - Premailer

For some users may be as simple as typing:

`gem install premailer`

in the terminal/shell.

[More info](https://github.com/premailer/premailer)

### 3 - Git

It's also recommended, but not mandatory, thay you [download and install git](http://git-scm.com/downloads/).

## Quick howto's 

### Generate html with Jeyll

In your terminal or shell:

`cd path/to/your/email/source/`

`jekyll build`

### In-linearize CSS with premailer

`cd path/to/your/email/output/`

`premailer index.html > linearized.html`

### Create A/B's

Use create git branches with A/B tests and merge the wining variants.
