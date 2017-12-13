# CV

This [Hexo](http://hexo.io) theme is designed for a CV. It's based on Cactus Light, a variant of Cactus Dark. I've modified the theme to make it suitable for a one-page CV that anybody can use. Thanks to [Pieter Robberechts](https://github.com/probberechts)' original work, and [Gabriela Thumé](https://github.com/gabithume)'s derivative theme, it's fully responsive. 

![](https://www.dropbox.com/s/hduj6dhlpsbqhbh/Screenshot%202017-12-13%2011.45.52.png?dl=1)

## Why?

I've moved countries a few times in the past few years, and worked freelance my entire adult life. I have to update my CV all the time! Previously, I'd keep a text file with all of my information, put this into InDesign, and make it look nice. Then I'd realise that I forgot something crucial, and edit my text file or the InDesign file directly. I ended up with different versions, and having to manually check that I hadn't copied text from a less-complete previous version.

In short, all of the type of problems that Git versioning can solve. This theme uses Hexo to take a series of MarkDown files for the various parts of my CV and turn them into simple HTML file which I can serve to the web. Now I only need to update one file, push it to GitHub, and the changes are live on the web.

[Demo](http://cv.olliepalmer.com)



## Summary

- [General](#general)
- [Features](#features)
- [Install](#install)
- [Configuration](#configuration)
- [License](#license)

## General

- **Version** : 2.0
- **Compatibility** : Hexo 3 or later

## Features

- Fully responsive
- Disqus
- Google analytics
- Font Awesome icons
- Pick your own code highlighting scheme
- Configurable navigation menu
- Projects list
- Simplicity

## Install
1. In the `root` directory:

    ```git
    $ git clone https://github.com/gabithume/cactus-light.git themes/cactus-light
    $ npm install hexo-pagination --save
    ```

2. Change the `theme` property in the `config.yml` file.

    ```yml
    # theme: landscape
    theme: cactus-light
    ```

3. Run: `hexo generate` and `hexo server`

## Configuration

If you want demo content, move the `_posts` folder from the `demo-content` into your `root/source` folder.


### Navigation

Setup the navigation menu in the theme's `_config.yml`:

  ```
  nav:
    Contact: /#contact
    Profile: /#profile
    Education: /#education
    Teaching: /#teaching
    Work: /#work
  ```
Note that the links must match the page titles of each page, as set in the page's meta-section:

```
---
title: contact
order: 1
---

## Contact
 
123 Street Avenue, Townsville, Country, XX12 3XX
Phone: +XX XXX XXXX

```

Note that the title becomes a div id, and the order determines where on the page the section comes. You can create new sections and edit the current ones as much as you like. 


## License
MIT
