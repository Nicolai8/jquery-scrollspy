# scrollspy.js

A jQuery plugin for detecting enter/exit of elements in the viewport when the user scrolls.

## Usage

```js
$('.tile').on('scrollSpy:enter', function() {
	console.log('enter:', $(this).attr('id'));
});

$('.tile').on('scrollSpy:exit', function() {
	console.log('exit:', $(this).attr('id'));
});

$('.tile').scrollSpy();

// or you could do this:
// $.scrollSpy($('.tile'));
// or this
// $('.tile').each(function(i, element) {
// 		$.scrollSpy(element);
// });

```

# Window Resize

Use the ```scrollSpy:winSize``` event for watching window resize.  This fires any time the window is resized by the user.

```
$.winSizeSpy().on('scrollSpy:winSize', funcy)
```
