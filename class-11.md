# EJS

## EJS stands for ***Embedded JavasScript Templating***

* EJS is a simple templaying language that lets you generate HTML markup with vanilla JavaScript.

* Important features for EJS:
1- Fast
2- Simple
3- Server JS and browser support

### Getting started

* To install it use command npm install ejs

* npm install --save express body-parser cors ejs

* To use it you need to pass an EJS template, first requiring the ejs database then adding the data.

* Do variables that require express,body-parse,path and cors.

* After you assign a var app= express();, you can app.use both bodyparser and cors then app.set ('views,path.join(__dirname,'views'))

* then app.set('view engine', 'ejs')

### Using it to create data

* create an index.ejs file with the tags you want.

* EJS symbol <%= foo %> inside the ejs file and after the respond.render isnide the function option, it will take the value of foo inside the object.

* We can use arrays to inject inside the page.

* Add <% %> and then put for loop inside it, for < var person of people >{ and then put inside the thing that u want inside and close the bracket with another <% } %>

* We can also use If statements, when a condition is met it inserts a specific value.
