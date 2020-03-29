# jQuery, Events, and The DOM

## JavaScript and jQuery book by Jon Duckett pages 293-301, 306-331 and 354-357

* jQuery is a JS file that lets you find elements using css-style selectors and then apply something using it's methods.

* jQuery has a simple way: select elements, perform tasks and handle events

* You can select element then apply methods to it with; ex: $('li.hot').addClass('complete');

* You can get jQuery as a file and link it or use a CDN link.

* Use jQuery because its simpler than javascript

## Get and set data

* You can get data by using for example var something = $('li).html() and you can set it by giving it an argument, like html('something')

* You can update multiple elements using one method instead of a loop like in vanilla javascript also known as **Implicit iteration**

* You must use the ready function for jquery to check that the page is ready for the code.

* A shorthand method is $(function() {
    //script goes here
});

* To add new element to page first you need to create it like: var $newFragment = $('< li >'), then use .before,.after etc etc...

* you can get attribute values by .attr(), remove the values by removeAttr(), add class by .addClass() and removeClass().

* You can also get and set CSS properties using .css(), you can set multiple properties using object literal notation.

* if you need to loop throught multiple element selections, you can use .each() method, you can access the current element using $(this)

* to apply event methods, you can use .on()

* You can load jquery from a cdn by including < script src=" //ajax .googl eapi s . com/ ajax/l i bs/ jquery / 1.10 . 2/ jquery .min. js "> < /script>

* You need to put the jQuery file or link right before the closing of the body tag.

## Pair Programming Reasons

* Pair programming has two main roles, the driver and the navigator, the driver is the programmer who types, while the navigator guides the driver and thinks about the big picture.

* Pair programming help you with efficiency, as two people working on the same problem can come with solutions faster than one person.

* It also helps with focusing, when two programmers work together they focus better.

* Learn from fellow students and colleagues, as you can see new problem solving methods and add them to your own.

* It improves your social skills since you work with another person who might have a different coding style.

* Job, interview and work environment readiness.



