1. There is subtle different between geting the dom object with javascrip and
jquery:
        javascrip just gives the element, but jquery gives that in array
        we can't use jqury methods on js objects.

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

5. Traversing the dom with jquery:

    a. $("#social-nav").next()
    b. $("#social-nav").prev()
    c. $("#social-nav").parent()
    d. $("#social-nav").parents()  all the parents and grand parents and ...
    e. $("#social-nav").children()
    f. $("#social-nav").find(".facebook")       find the element in the #soical nav with 
                                                that selector  
6. We can use chaining in jquery

7. We can add content by this functions:
  a. $("#tweets").append("<div></div>"); at the end of element
  b. $("#tweets").prepend("<div></div>"); at the first of element
  c. $("#tweets").before("<div></div>"); before the element
  d. $("#tweets").after("<div></div>"); after the element
  e. $("#tweets").html("<div></div>"); replace all the content in it
  f. $("#tweets").text("<div></div>"); just change the text

     
  
  

     
    






