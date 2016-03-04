# Pasteque-catalog
jQuery based catalog application. This is a learning application made for PopSchool, Valenciennes FR. See http://pop.eu.com/popschool
It uses Pastèque (see http://www.pasteque.coop) API.

Pastèque’s API is here : http://redmine.scil.coop/projects/pt-server/wiki/Api_doc7
We use demo account of Pastèque’s hosting service : https://my.pasteque.coop with demo6 as login and password

This application aims to list all the products of a given catalog in Pastèque and display detailled information about them.

#Step by step procedure

## Create the scaffold
Create one empty HTML file with jQuery and bootstrap
Add one div with id categories, one div with id products and one div with id products, one div with id product-details

## jQuery get of categories
On document ready, make a request to get all categories.
- Try the request in your browser
- Use $.getJSON to get the categories
- Put the result in the div.categories, one div for a category. div id is category id. Display category's name
- Add a sub-request to get the category’s image if any, display this image in the div

## jQuery get of products
Make a function called when a category’s div is clicked
- Try a request on a category in your browser
- Empty the content on div.products
- Put the result in div.products, one div for a product. div id is product id. Display product’s label
- Add a sub-request to get the product’s image if any, display this image in the div
- keep all the data in a variable

## show Product
Display data about a product when a product’s div is clicked
- Display an image for the bar code with barcode-coder’s jquery library : http://barcode-coder.com/
