## include css and js
my assume you have include jquery.js

```html
<link href="vendor/magnific-popup/magnific-popup.css" rel="stylesheet"> 
<script src="vendor/magnific-popup/magnific-popup.js"></script>
``

## install plugin

```js
    // The magnific popup jQuery plugin
  $('.down-popup').magnificPopup({
    type: 'image',
    removalDelay: 300,
    mainClass: 'mfp-fade',
    gallery: {
      enabled: false
    },
    zoom: {
      enabled: true,
      duration: 300,
      easing: 'ease-in-out',
      opener: function (openerElement) {
        return openerElement.is('img') ? openerElement : openerElement.find('img');
      }
    }
  });
```

## set in html
add class that you set when install in href. My case is down-popup.

```html
<a href="img.jpg" class="down-popup"><img src=" img.jpg"></a>
```
