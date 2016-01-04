This is simple pulse counter with redirection to some url using jQuery

gjCountAndRedirect( (int)numberOfSecounds, (string)urlToRedirectTo );

Example of use:
On click:
https://jsfiddle.net/GlupiJas/k6prgpbw/

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

On load:
https://jsfiddle.net/GlupiJas/r29r1h0c/

// USE EXAMPLE
$(document).ready(function() {
  gjCountAndRedirect(10, document.URL);
}
