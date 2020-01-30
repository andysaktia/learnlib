
## in html
```html
<a href="img.jpg" class="down-popup"><img src=" img.jpg"></a>
```

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
