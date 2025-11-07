# Tech writing webring 

A simple, static webring service linking blogs that are related to tech writing

## What is a webring?

A webring is a collection of websites linked together in a circular structure. Visitors can navigate through the ring by clicking "next" or "previous" links, discovering new sites along the way.

## Features

- Clean, minimal design with Pico CSS
- Easy navigation between member sites (previous, next, random)
- Fully responsive and mobile-friendly
- Zero dependencies - pure HTML, CSS, and JavaScript
- Simple link-based navigation (no JavaScript required on member sites!)

## Add your site

To add your site to the webring:

1. Fork this repository
2. Add your site to `sites.json`
3. Add the webring links to your site (see below)
4. Submit a pull request

### Add webring links to your site

Simply add these HTML links anywhere on your site:

```html
Part of the <a href="https://caseyrfsmith.github.io/webring/">tech writing blog webring</a> | 
<a href="https://caseyrfsmith.github.io/webring/navigate.html?action=prev&site=YOUR-SITE-URL">Previous</a> | 
<a href="https://caseyrfsmith.github.io/webring/navigate.html?action=next&site=YOUR-SITE-URL">Next</a> | 
<a href="https://caseyrfsmith.github.io/webring/navigate.html?action=random&site=YOUR-SITE-URL">Random</a>
```

Replace `YOUR-SITE-URL` with your actual site URL (e.g., `https://example.com`). Feel free to just use the first line (Part of the...). This doesn't need to be serious :).

## File structure

```
.
├── index.html          # Main webring hub page
├── navigate.html       # Navigation handler (redirects to prev/next/random)
├── sites.json          # Member sites data (JSONP format)
└── README.md           # This file
```

## License

This project is released into the public domain. Feel free to use, modify, and distribute as you wish.