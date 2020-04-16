# Overview:

A tutorial based app to demonstrate Rails with JQuery functionality

JQuery added through yarn install for Rails 6.0.2.2 used in this repo.
Instructions followed as explained in this website:
https://www.botreetechnologies.com/blog/introducing-jquery-in-rails-6-using-webpacker

### Version used:
* Ruby version -> 2.6.5p114

* Database creation -> created through hard coding in seeds.db

## Resources: 
https://www.botreetechnologies.com/blog/introducing-jquery-in-rails-6-using-webpacker

and this awesome tutorial that just walks you through the whole thing, easily:

https://blog.engineyard.com/using-jquery-with-rails-how-to

### Errata:
There is an error in the engineyard tutorial (small oversight).  The code below:

```
$(document).ready(function() {
  $('[data-js-hide-link]').click(function(event){
    alert('You clicked the Hide link');
    event.preventDefault(); 
  });
}
```

misses an end parantheses ) and doesn't work. Please use this instead:

```
$(document).ready(function() {
  $('[data-js-hide-link]').click(function(event){
    alert('You clicked the Hide link');
    event.preventDefault(); 
  });
});
```
