# Thor

![Ghost version](https://img.shields.io/badge/Ghost-0.7.x-brightgreen.svg?style=flat-square)
[![Donate](https://img.shields.io/badge/donate-paypal-003087.svg?style=flat-square)](https://www.paypal.me/andreatarquini/5)

> A simple theme for Ghost made for geeks, hackers and developers (forked from Casper).

I made some small but essential modifications. More changes to come, first of which will be to adapt to newer Casper.

## Intro
**Thor** is a very simple fork of the [Odin](https://github.com/h4t0n/odin)
theme, which is a fork of [Casper](https://github.com/TryGhost/Casper), the Ghost default theme.

I, Douglas modified Andrea's Odin to fit my needs for a portfolio theme. More changes planned.

Some key changes are that home page only displays featured posts, so you can curate your portfolio while still having other content elsewhere on the site.

I also removed unnecessary sharing buttons like Gplus.



### Features
* Casper minimalistic and clean style (without right side menu)
* Works with Ghost 0.7+
* Fully responsive (for mobiles and tablets)
* Home Page Navigation Menu Buttons
* Google Analytics (easily configurable by code injection in the admin area)
* [Disqus](https://disqus.com) comments (easily configurable by code injection in the admin area)
* [Prism](http://prismjs.com/) Syntax Highlight (all languages supported)
* [RRSSB](https://github.com/kni-labs/rrssb) Extraordinary Social Sharing Buttons
* [Font Awesome](http://fontawesome.io) home page Social Link Icons (easily configurable by code injection in the admin area)

### Demo
I've created and I use this theme for my personal blog at [blog.h4t0n.com](https://blog.h4t0n.com).

## Installation
Installation is the same as other themes, so clone or download the content of this repo inside your Ghost `content/themes/` folder.

```
# for example
$ cd /your-ghost-root-directory
$ git clone https://github.com/h4t0n/odin.git content/themes/odin
```

Restart Ghost and select Odin theme from your Admin Area.

## Configuration
No need to configure ***Prism*** or ***RRSSB*** buttons.

To add Homepage Navigation Menu Buttons simply add the links in your Navigation Admin Area. They may be useful for static pages (*AboutMe* for example) or for shortcut to your (best) post tags.  

Odin comes with a default ***favicon*** generated with [Real Favicon Generator](http://realfavicongenerator.net). If you want to add your *favicon* you can generate your own (with [Real Favicon Generator](http://realfavicongenerator.net)) and place downloaded files inside the ***assets/img/favicons*** Odin directory.

***Disqus*** comments, ***Google Analytics***  and ***Font Awesome Home Page Social Link Icons*** are disabled by default, but they are easily configurable with *Blog Header Code Injection* inside your Ghost Admin Area.

```html
<script>
// to enable Google Analytics
var ga_id = 'YOUR-UA-ID_HERE';

// to enable Disqus
var disqus_shortname = 'YOUR_DISQUS_SHORTNAME'


// to enable Social Link Icons add the social_link object
// with the pair key/value -> social_network/link
// NB: the key is used to include the right icon from Font Awesome
// (you can include any Font Awesome icon)

// Example1: default social network icons
var social_link = {
    'twitter': 'https://twitter.com/h4t0n',
    'linkedin': 'https://it.linkedin.com/in/andreatarquini',
    'github': 'https://github.com/h4t0n',
    'rss':'https://blog.h4t0n.com/rss/'
    // you can add more icons
}

// Example2: squared social network icons
var social_link = {
    'twitter-square': 'https://twitter.com/h4t0n',
    'linkedin-square': 'https://it.linkedin.com/in/andreatarquini',
    'github-square': 'https://github.com/h4t0n',
    'rss':'https://blog.h4t0n.com/rss/'
    // you can add more icons
}

</script>


```


## Copyright & License

Released under the MIT License.  
Copyright (c) 2018 [Douglas Hewitt](https://madebydouglas.com) [@madebydouglas](https://twitter.com/madebydouglas)  
Copyright (c) 2013-2018 Ghost Foundation (for Casper theme substantial portions of code)
