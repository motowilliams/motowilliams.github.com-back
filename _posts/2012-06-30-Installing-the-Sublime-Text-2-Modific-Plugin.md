---
layout: post
image_root: "/assets/images/"
title: "Installing the Sublime Text 2 Modific plugin"
author: "Eric Williams"
categories: [code]
---

There really isn't enough nice things to say about [Sublime Text 2](http://www.sublimetext.com/).  It is a nice [cross platform minimalist text editor](http://www.sublimetext.com/2) that seems to get things right.  You can even install it Dropboxable aka Portable.  So run, don't walk over to Crazy Larry's House of Editors and [get you some editor joy](http://www.sublimetext.com/buy).   

Since you are probably working on a [source file or two some of some flavor or another](https://github.com/languages/) you are probably using with source control.  This will be the case if the file is important to you but we're not here today to talk about that.  For the intent of this post you are using [git](http://git-scm.com/) and you are interesting in some lightweight status of your changes in-flight.

[Oren Farhi (@orizens)](https://twitter.com/orizens) has a nice write up on what the [Modific](https://github.com/gornostal/Modific#readme) [plugin does](http://orizens.com/wp/topics/sublime-text-modific-plugin-changes-since-last-commit/).  Go read that for the 'what it gives you' and we will finish up when you get back.

## Install it already ##

Sublime Text 2 and its [Sublime Package Control](http://wbond.net/sublime_packages/package_control) make this very easy.

1. Open subl
2. Open the Sublime Text 2 console.  **View > Show Console** or **Ctrl+`**
3. Paste the following (from [Sublime Package Control installation](http://wbond.net/sublime_packages/package_control/installation)): 

> import urllib2,os; pf='Package Control.sublime-package'; ipp=sublime.installed_packages_path(); os.makedirs(ipp) if not os.path.exists(ipp) else None; urllib2.install_opener(urllib2.build_opener(urllib2.ProxyHandler())); open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read()); print 'Please restart Sublime Text to finish installation'

4. Restart subl
5. Open the Command Pallete aka package manager by **Tools > Command Palette** or **Ctrl+Shift+P**
6. Type in **Package Control: Install Package** and press enter.  The package list will refresh
7. Type Modific and press enter
8. Restart subl
9. Open a file that is in a git repository
10. Profit!