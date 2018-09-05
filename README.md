# Potato Dark [![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/surajmandalcell/potato-dark/blob/master/license.md) 

Outrun with the power of a potato. Based on the Potato Dark theme with CSS bits inspired by Dusk.

![screenshot](https://github.com/surajmandalcell/potato-dark/blob/master/images/screenshot.png)   

## Overview

* Support for tags
* Responsive design
* Support for Related Content
* Analytics with Google Analytics
* Modern, Simple and beautiful design
* Medium's Image Zoom（[zoom.js](https://github.com/fat/zoom.js/))
* Social links （most social networks available）
* Inlined CSS for customizable colors via config.
* Outrun inspired foreground colors on a dark background, by default.
* Can turn of pagination.

Use short code for Image Zoom.

```
{{% zoom-img src="/images/default.jpg" %}}
```

## Installation

cd your hugo site directory and run:

```shell
$ mkdir themes
$ cd themes
$ git submodule add https://github.com/VVelox/hugo-dusky-neon-potato.git dusky-neon-potato
```

## Usage

Use hugo's -t dusky-neon-potato or --theme=dusky-neon-potato option with hugo commands. Example:

```shell
$ hugo server -t dusky-neon-potato -w -D
```

## Configuration

### Disable Pagination

So lets say you have a page you don't want pagination displayed, such as "About.org",
then you can set <code>no_pagination</code> to true in the Front Matter and it won't
display.

```
---
title: "About"
date: 2018-09-02T22:41:40-05:00
draft: false
no_pagination = true
---

A rutting about page.
```
