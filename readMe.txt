1. There is subtle different between geting the dom object with javascrip and
jquery:
        javascrip just gives the element, but jquery gives that in array
        we can't use jqury methods on js objects.

///// Getting elements //////

2. We can get elements by $("css selectors")

3. We can give css styles $("css selectors").css({border: 3px solid blue});

4. Using filters for more specific selection:
    a. select first and last: 
    $("header nav li:first")
    $("header nav li:last")

    b. select if they are first child or last child:
    $("header nav li:first-child")
    $("header nav li:last-child")

    c. find the even ones:
    $("header nav li:even")
    
    d. not filter:
    $("section:not('#contact')")

    e. less than and greater than:
    $("header nav li:lt(3)")
    $("header nav li:gt(3)")

    f. attribute selector:
    $("img[alt=quote]")

////////// Traversing the dom ///////
5. Traversing the dom with jquery:

    a. $("#social-nav").next()
    b. $("#social-nav").prev()
    c. $("#social-nav").parent()
    d. $("#social-nav").parents()  all the parents and grand parents and ...
    e. $("#social-nav").children()
    f. $("#social-nav").find(".facebook")       find the element in the #soical nav with 
                                                that selector  
6. We can use chaining in jquery

//////// Adding & removing contents ///////

7. We can add content by this functions:
  a. $("#tweets").append("<div></div>"); at the end of element
  b. $("#tweets").prepend("<div></div>"); at the first of element
  c. $("#tweets").before("<div></div>"); before the element
  d. $("#tweets").after("<div></div>"); after the element
  e. $("#tweets").html("<div></div>"); replace all the content in it
  f. $("#tweets").text("salam"); just change the text

  g. empty() - empty the inner HTML of an element
  h. remove() - removes the element completely
  
////// Wrapping and uwrapping /////////

8. wrapping means adding parent element for a element
     
     a. $("section").wrap("div"); wrap the element with div
     b. $("section").unwrap();
     c. $("section").wrapAll("div") wrap all the elements in 
     a div tag

/////// Attributes & CSS and classes ////
9. Changing the attribute:

.removeAttr("alt");
.attr("alt", "location"); (setting attributes)
.attr("alt");      (reading attributes)

10. working with CSS in jquery:

$("").css("color");    Reading the css value for color
$("").css("color,"red"); Setting the color to red;
[ATTENTION]
We can also pass json objects to css:
$("").css({
  "top":50px,
  "opacity": 0.2,
  "border-top": "1px solid red"
})

11. Working with classes in jquery:

$("").removeClass("");   it remove the clss from an element
$("").addClass("");      it add class to an element
$("").toggleClass("");   it add class if it doesn't exist or
remove class if it exist

/// Events in jquery ///////

12. we can use jquery to Bind and Unbind events handlers:

$("").on("click", function(e){
  $(this).css("background", "pink");
});
$("").off("click");

13. Event helpers in jquery:
$("").click(function(e){                   .click() is same as .on("click", function(){})
  $(this).css("background", "pink")
})

14. To move the script tag at top of the page use:
      $(document).on("ready", function(e){})
      $(document).ready(function(){})
      $(function(e){})
or    document is just for elements, window for example is
consider images to
      $(window).on("load", function(e){})

15. We can use e.stopPropagation(); for stopping event bubbling
  a. e.type             shows the event type
  b. e.target           shows the target element
  c. e.pageX            show the x coordination


///////// Jquery animations /////////

16. We can use animate instead of css function for numerical 
values:
$(this).animate({
  "height": "200px",
  "width": "500px"
}, 1000, "linear" or "swing", function(){}) 

17. We can use animate for fading elements:
  a. $(this).animate({"opacity": "0.5"}, 1000);

18. Or we can use fade*() function to change the opacity
  b. $(this).fadeOut(1000, function(){});      this function remove the element from dom
  c. $(this).fadeIn(2000, function(){});
  d. $(this).fadeTo(2000, 0.2);

19. OR we can use (it changes in how the element hide or show):
    a. $().hide(1000, function(){});
    b. $().show(1000, function(){});
    c. $().toggle(1000, function(){});     (hide or show depends on curent state)

20. We can use slideUp() or slideDown() to change the height
to zero or initial height:
    a. $().slideUp(1000, function(){});
    b. $().slideDown(1000, function(){});
    c. $().slideToggle(1000, function(){});

21. We can use jquery plugins:
  responsiveSlides.js

     
    






