<h1>This is simple pulse counter with redirection to some url using jQuery</h1>
```javascript
var numberOfSecounds = 10;
var urlToRedirectTo = "http://google.com";
gjCountAndRedirect(numberOfSecounds, urlToRedirectTo );
```

Example of use:
On click:
https://jsfiddle.net/GlupiJas/k6prgpbw/

```javascript
// USE EXAMPLE
$(document).ready(function() {
  //var
  var gjCountAndRedirectStatus = false; //prevent from seting multiple Interval

  //call
  $('h1').click(function() {
    if (gjCountAndRedirectStatus == false) {
      gjCountAndRedirect(10, document.URL);
      gjCountAndRedirectStatus = true;
    }
  });

});
```

On load:
https://jsfiddle.net/GlupiJas/r29r1h0c/
```javascript
// USE EXAMPLE
$(document).ready(function() {
  gjCountAndRedirect(10, document.URL);
}
```
