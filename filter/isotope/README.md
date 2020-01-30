  [isotope-site](https://isotope.metafizzy.co/)
  
  ## install in js
  ```js
  
  // Porfolio isotope and filter
  var portfolioIsotope = $('.portfolio-container').isotope({
    itemSelector: '.portfolio-item',
    layoutMode: 'fitRows'
  });

  $('#portfolio-flters li').on( 'click', function() {
    $("#portfolio-flters li").removeClass('filter-active');
    $(this).addClass('filter-active');

    portfolioIsotope.isotope({ filter: $(this).data('filter') });
  });
  
  ```

## practice in html
data-filter handle class container that have define, example class name `.Category`, for all item you can use `*`.
class filter-active in tag li make display possible to show.

```html
  <li data-filter=".Category" class="filter-active"><?= $item['name'];?></li>
  <!-- BLOCK THAT WILL BE FILTER-->
  <div class="row portfolio-container">
    <div class="col-lg-4 portfolio-item Category">
        <div class="portfolio-wrap">
            <figure>
                <img src="<?= $image ;?>" class="img-fluid" alt=""> 
            </figure> 
        </div>
     </div> 
  </div>
```
