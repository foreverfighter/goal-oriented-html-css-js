# goal-oriented-html-css-js

Start with a goal, and learn how to do it here.

# Goals

<!-- META -->
  <!-- ENABLE TOOLS -->
  <!-- WORK WITH ECOSYSTEM -->
<!-- CONTENT -->
<!-- LAYOUT -->

## Content

1.  [Create a header](#create-a-header)
2.  [Use localStorage to store data](#use-localstorage-to-store-data)

## Layout

3.  [Vertically and horizontally center an element](#vertically-and-horizontally-center-an-element)

## Metadata

### Work with the internet ecosystem

4.  [Make a webpage](#make-a-webpage)
5.  [Add a title](#add-a-title)
6.  [Add a favicon](#add-a-favicon)
7.  [Add a stylesheet](#add-a-stylesheet)
8.  [Use English as the main language](#use-english-as-the-main-language)
9.  [Use utf-8 character encoding](#use-utf-8-character-encoding)
10. [Provide cross-browser default styling consistency](#provide-cross-browser-default-styling-consistency)
11. [Add mobile-responsiveness](#add-mobile-responsiveness)
12. [Improve your SEO](#improve-your-seo)
13. [Add metadata for web mobile apps](#add-metadata-for-web-mobile-apps)

### Enable common tools

14. [Add Bootstrap](#add-bootstrap)
15. [Add Google Analytics tracking](#add-google-analytics-tracking)

### Vertically and horizontally center an element

```
.parent {
  display: flex;
  align-items: center;
  justify-content: center;
}
```

show inputs
show text
show images
create links
create lists
create tables
make elements draggable
make screen responsive
assign javascript on events(use oninput for input)

re styles: line-height is important for y-position of text

define colors
define fonts
define layout
define position
use media queries
use support queries
create image filters
create animations
create counter
draw shapes

### create image filters

```
/* simple filter */
.myElement {
    -webkit-filter: blur(2px);
}

/* advanced filter */
.myElement {
    -webkit-filter: blur(2px) grayscale (.5) opacity(0.8) hue-rotate(120deg);
}
```

### create animations

```
.slider {
    overflow-y: hidden;
    max-height: 500px; /* approximate max height */

    transition-property: all;
    transition-duration: .5s;
    transition-timing-function: cubic-bezier(0, 1, 0.5, 1);
}
```

### create counter

```
ol.toc, ol.toc ol {
    counter-reset: toc;
}
ol li {
    counter-increment: toc;
}
.toc li:before {
    content: "(Item " counters(toc, ".") ")";
}
```

### draw shapes

```
.circle {
    border-radius: 50%;
    width: 200px;
    height: 200px;
    /* width and height can be anything, as long as they're equal */
}
```

## Make a webpage

Add `<!DOCTYPE html>` to the top of the file and wrap your text in `<html>` tags.
Also, add `<head>` and `<body>` tags.

```
<!DOCTYPE html>
<html>
  <head>
  </head>
  <body>
  </body>
</html>
```

## Use English as the main language

```
<html lang="en" dir="ltr">
</html>
```

## Use utf-8 character encoding

https://www.fileformat.info/info/unicode/utf8.htm

```
<head>
  <meta charset="utf-8">
</head>
```

## Provide cross-browser default styling consistency

Download here: http://necolas.github.io/normalize.css/
Read about it: http://nicolasgallagher.com/about-normalize-css/

```
<head>
  <link rel="stylesheet" href="css/normalize.css">
</head>
```

## Add a title

```
<head>
  <title>My Title</title>
</head>
```

## Add a favicon

Upload a favicon.ico into the root directory on the server hosting your web page.

See: https://www.computerhope.com/issues/ch000410.htm

Create a favicon.ico: https://www.favicon-generator.org/

OR if your page is meant for local use, use the below.

```
<head>
  <link rel='shortcut icon' type='image/x-icon' href='/favicon.ico' />
</head>
```

## Add a stylesheet

```
<head>
  <link rel="stylesheet" href="css/main.css">
</head>
```

## Add Bootstrap

Download: http://getbootstrap.com/.

```
<head>
  <link rel="stylesheet" href="css/bootstrap.min.css">
</head>
```

## Add mobile-responsiveness

This adjusts the width of the page to fit the width of the device's screen.

```
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1">
</head>
```

## Improve your SEO

```
<head>
  <meta name="description" content="Show pictures of cute rabbits">
</head>
```

## Add metadata for web mobile apps

```
<head>
  <link rel="manifest" href="/manifest.webmanifest">
</head>
```

## Add Google Analytics tracking

Replace `'GA_TRACKING_ID'` below with your [tracking ID](https://support.google.com/analytics/answer/1008080?hl=en).

```
<!-- Global Site Tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'GA_TRACKING_ID');
</script>
```

## Create a header

Enclose text with <h1> and </h1>.

```
<h1>hello world</h1>
```

## Use localStorage to store data

```
<!-- Store data -->
localStorage.setItem("lastname", "Smith")

<!-- Get data -->
localStorage.getItem("lastname")
```
