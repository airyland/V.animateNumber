# 演示文档

---

<style>
#test,#test2,#test3 {font-family:'Open Sans';font-size:25px;font-weight:600;}
</style>

<div id="test"></div>

<div id="test2"></div>

<div id="test3"></div>


````javascript
seajs.use('animateNumber', function(animateNumber){
      var $ = jQuery;
      animateNumber(jQuery);
      $("#test").animateNumbers(1234, false, 2000, "linear");
      $("#test2").animateNumbers(1234, true, 2000); // two second swing with commas
      $("#test3").animateNumbers(4321); // one second swing with commas
});
````



