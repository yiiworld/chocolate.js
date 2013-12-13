Chocolate.js
============

Chocolate.js is a high-customizable pop-up gallery.

## API

Inlcude Chocolate styles and script:

```html
<link href="/css/chocolate.css" rel="stylesheet">
<script src="/js/chocolate.js"></script>
```

Then create new instance of chocolate passing HTMLCollection to it:

```html
<script>
  new chocolate(document.querySelectorAll('img'));
</script>
```

Chocolate automatically added all images you've passed to his gallery. Then when you click on one of this images, chocolate open the image in its gallery. You can switch between images by clicking on them thumbnails or by pressing arrow keys or by clicking on panels.

## Themes

Chocolate consists of four different zones: thumbnails, container with image, left panel, right panel. You can manage actions which occur when you click on one of three zones (exclude thumbnails).

You can create your own
 * stylesheets,
 * images,
 * templates,
 * options.

## Build your own Chocolate

To create your own build exec

```
$ cake build
```

Options:

```
  -t theme      name of theme [default]
  -b path       basedir for theme images [/dist/default/images]

  --no-touch    compile without touch support
  --no-history  compile without history api support
  --no-session  compile without sessionStorage support
```

Example:

```
$ cake -t simonenko.su -b /i/chocolate/ --no-touch build
```
