#Install

include css
<link rel="stylesheet" href="owlcarousel/owl.carousel.min.css">
<link rel="stylesheet" href="owlcarousel/owl.theme.default.min.css">

include js
<script src="jquery.min.js"></script>
<script src="owlcarousel/owl.carousel.min.js"></script>

set HTML
<!-- Set up your HTML -->
<div class="owl-carousel">
  <div> Your Content </div>
  <div> Your Content </div>
  <div> Your Content </div>
  <div> Your Content </div>
  <div> Your Content </div>
  <div> Your Content </div>
  <div> Your Content </div>
</div>

call the plugin
$(document).ready(function(){
  $(".owl-carousel").owlCarousel();
});
