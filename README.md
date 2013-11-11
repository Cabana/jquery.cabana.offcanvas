# jQuery OffCanvas nav plugin

jQuery OffCanvas nav plugin is for adding off canvas (facebook) style naviagation to a web page.

## Dependencies
* jQuery library
* jQuery UI Core library
* Zurb Foundation CSS library (optional)
* FastClick - https://github.com/ftlabs/fastclick
* Modernizr (custom build with `Modernizr.prefixed()`)

## Usage
Include `cabana.offcanvas.js` in your JS (app.js) bundle.
To add Off Canvas navigation, make a div with an id `off-canvas`. All other page content should go below.
```html
<body>
	<div id="off-canvas">
		<p>Your off-canvas navigation here</p>
	</div>
	<header>Page header</header>
	<section>Page section</section>
	<footer>Page footer</footer>
</body>
```
and initiate it through javascript:
```js
$(document).ready(function(){

	$(document).offcanvas();

});
```

## Options
* `navOpenBtn` - any html element selector (ie. `".nav-open-btn"`)
* `navCloseBtn` - any html element selector (ie. `".nav-close-btn"`)
* `pageRoot` - default `"body"`. Sets the root element for the off canvas nav. Set this only if you must
* `offCanvasContainerId` - Element id. See usage at the top. For example: `"off-canvas"`
* `_outerWrapId` - Element id. Off canvas outer wrapper. Only if you must
* `_innerWrapId` - Element id. Off canvas inner wrapper. Only if you must

## Methods
* `toggleNav` Opens/Closes navigation. If attached to a anchor element, pass event as a second param.

### Compatibility
IE9+, all modern browsers

### Tips and tricks
See `examples` folder for extended customization
