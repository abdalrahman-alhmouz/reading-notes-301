# Components - EJS Partials

* Partials are like a function for reusing same HTML across multiple pages.

* Ypu cam use the same partials in different page using include function and then add it wherever you need it to be added to.

* We can use that for repititive elements such as header and footer.

* You can create partial files inside **views/partials/nameOfThing.ejs** and that file will contain only the thing that you want to reuse, like a navigation bar for example.

* Now we can use that file inside other HTML files by including them in the strawberry tags

* You can include a partial file with <%-include(partial_file_name)%> where you insert partial file name.

* And its that simple how we can easily add chunks of reusable elements using EJS,express and NodeJS!
