# Image Map Resize

*This is a simple library that makes HTML Image Maps responsive, so that they automagically stay scaled to the size of the image they are attached to. It detects the window being resized and updates the co-ordinates of the image map accordingly.*

*This library can be used with or without jQuery.*

### Native JS Usage

Inclue the [imageMapResizer.min.js](https://raw.github.com/davidjbradshaw/imagemap-resizer/master/js/imageMapResizer.min.js) srcipt then add the following call to the bottom of your page:

```js
imageMapResize([selector || map object]);
```

Optionally you can pass a CSS selector that returns a collection of map tags, for example 'map.myMap'. Or a direct reference to a map object in the DOM.


### jQuery Usage

Inclue [jQuery](http://jquery.com) and the [imageMapResizer.min.js](https://raw.github.com/davidjbradshaw/imagemap-resizer/master/js/imageMapResizer.min.js) script and then add the following call to the bottom of your page:

```js
$('map').imageMapResize();
```

Or you may want to wrap it in a `$(document).ready()` function:

```js
$(document).ready(function() {
    $('map').imageMapResize();
});
```

###Example
http://davidjbradshaw.com/imagemap-resizer/example/

### A note on IE8 and below

To use this library with old IE you will need to also load the included polyfil and ensure IE is running in "[Standards mode](http://en.wikipedia.org/wiki/Internet_Explorer_8#Standards_mode)". This can be done by adding the following to your HTML head section.

```html
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<!--[if lte IE 8]>
	<script type="text/javascript" src="js/ie8.polyfil.min.js"></script>
<![endif]-->
```

[![NPM](https://nodei.co/npm/image-map-resizer.png)](https://nodei.co/npm/image-map-resizer/)

### License
Copyright &copy; 2014 [David J. Bradshaw](https://github.com/davidjbradshaw).
Licensed under the [MIT license](http://opensource.org/licenses/MIT).
