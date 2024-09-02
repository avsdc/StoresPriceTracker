**Description:**

This project consists of two parts. Part1 uses Beautiful Soup, and Part2 uses Selenium.

In the first part, get() function is used to retrieve information in the form of responses from the product web page. 
A Beautiful Soup object soup is created by passing the product web page, and html.parser to the BeautifulSoup class.
The find() method of soup object is used to scrape information from the web page.
A product dictionary called product_dict is created where the logo, name of product, price of product and image are
passed as values to the product_dict. The product_dict is created for each product from each company i.e. Walmart,
eBay, and Amazon.
Each product_dict is added to a productList. There are 18 product_dicts for 18 products (six for each company - these
are laptop desk bed tray table, mobile phone, mattress, lawnmower, refrigerator, and luggage).


With the app.route("/"), and home() function, program navigates to the index.html page, and displays information
for each company and product.


In the second part, three new productLists are created. These are companyList, namesList, and pricesList and returned from
the function.

A Google form is created, and 3 questions are added to the form. These questions require short responses regarding the
company name, product name, and price of the product. A for loop that runs 18 times, for 18 products (six for each company)
is used. Selenium locates the areas to insert responses using find_element() and XPATH. These are the company_area, name_area,
and price_area. Once the responses are entered, submit_btn and print_another_response_btn are clicked, so that product information
for all 18 products is received. When this is completed, click on the Google spreadsheet icon, and inofrmation is inserted into
the Google spreadsheet.

**Requirements:**
Flask, BeautifulSoup, Selenium

**Usage:**
The webscraper project was created in Pycharm community Edition. Run the program in Pycharm, and first the index.html page
will be displayed with product information for 18 products from 6 companies.
Then, Selenium opens up the Google form, and automatically enters responses to the three questions (company name, product name, and price)
for all 18 products.
After all responses are entered, click on the icon for Google Spreadsheet, and all the responses will be entered on the spreadhseet.
