# animateNumber

---

数字递增动画

---

## 使用说明


## API

```javascript
$(el).animateNumbers(stop, commas, duration, ease);
```

参数说明：

+ `stop` (number): number to stop on
+ `commas` (boolean): turn commas on/off (default is true)
+ `duration` (number): how long in ms (default is 1000)
+ `ease` (string): type of easing (default is "swing", others are avaiable from jQuery's easing plugin


## 演示

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