---
layout: post
title: install jekyll in ubuntu
description: "jekyll install ubuntu"
categories: other
date: 2013-10-24
---

## synopsis
Building this blog in github use jekyll.TO easy preview the md file, so try to install jekyll local. 

## the process of install

1. **ubuntu**

    Sure `curl` exist in you system by `curl --version`.if not,excuting `sudo apt-get install curl` to install.
    For RVM to work properly, we  have to set the 'Run command as login shell' checkbox on the Title and Command tab inside of gnome-terminal's Settings page. Intergrating RVM with gnome-terminal,follow [this instruction](https://rvm.io/integration/gnome-terminal) to config.  
2. **ruby** 

    Before install ruby we need RVM. Excuting `curl -L https://get.rvm.io | bash -s stable` to get.  
    Then installl ruby by rvm `rvm install 2.0.0`.  
    Set the installed ruby as default version `rvmuse ruby-2.0.0-p247 --default`.  
    Change the gem source from default to [http://ruby.taobao.org](http://ruby.taobao.org) by the follow command  
    `gem sources --remove http://rubygems.org/`  
    `gem sources -a http://ruby.taobao.org/`  
    Now we excute `gem suorces -l` and we would see that  
    `*** CURRENT SOURCES ***`  

    `http://ruby.taobao.org/`  

3. **jekyll**

    Excuting `gem install jekyll` to install jekyll.  
    After completed input `jekyll -v` in terminal if failed,you need to add it to path  
    `PATH=$HOME/.rvm/gems/ruby-2.0.0-p247/bin:$PATH`  
    input `jekyll -v` again get  
    `jekyll 1.2.1`




