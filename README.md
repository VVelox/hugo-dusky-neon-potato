# Dusky Neon Potato [![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://raw.githubusercontent.com/VVelox/hugo-dusky-neon-potato/master/LICENSE.md)

Outrun with the power of a potato. Based on the Potato Dark theme with CSS bits inspired by Dusk.

![screenshot](https://raw.githubusercontent.com/VVelox/hugo-dusky-neon-potato/master/images/screenshot.png)

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
* Can turn off pagination.
* The ability to enable sorting of tables for pages.

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

### Sortable Tables

So lets say you want to make the tables on a page sortable, you can now do this.
You can do this, by setting the Front Matter value "sort_tables" to true and in
the header it will include a link to a JS script in the js dir that does this.

Below is a org mode example with sortable tables.

```
---
title: "Tables"
date: 2018-09-02T22:41:40-05:00
draft: false
sort_tables: true
---


| a | b | c          | d            | e |
|---+---+------------+--------------+---|
| 1 | f | 2017-03-14 | 127.0.0.1    |   |
| 2 | b | 2018-02-14 | 192.168.15.2 |   |
| 3 | e | 2017-03-15 | 192.168.1.1  |   |
| 4 | d | 2012-03-14 | 10.10.10.10  | 3 |

```

### Colors

All colors stuff go under

```
[colors]
	#general text and background
	text="#66FF00"
	background="#101010"
	# titles
	main="#FF1493"

	# headers
	h1="#FF00FF"
	h1-decoration="none"
	h2="#DA70D6"
	h2-decoration="none"
	h3="#EE82EE"
	h3-decoration="none"
	h4="#8B008B"
	h4-decoration="none"
	h5="#9932CC"
	h5-decoration="none"
	h6="#800080"
	h6-decoration="none"

	# tables
	table-border="#008B8B"
	th-bg="#3B0072"
	th-fg="#FF040C"

	# content tags
	ctag="#FF00FF"
	ctag-hover-fg="#66FF00"
	ctag-hover-bg="#101010"

	# color of the tags title on that tags page
	p-tag-title="#FF1493"

	# related items(at the cottom of posts)
	related-bg="#101010"
	related-fg="#66FF00"
```
