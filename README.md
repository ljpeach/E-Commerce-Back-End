# E-Commerce-Back-End
The back end for an e-commerce website. Integrates a MySQL database using ORM and provides multiple HTTP request api paths for interacting with the server. 

## Installation Guide

1. Download the repository using your favorite method (git clone, download as zip, etc.).
2. Open a terminal instance in the `E-Commerce-Back-End` directory.
3. Call ```npm i``` and wait for dependant packages to install.
4. Start instance of MySQL CLI using ```mysql -u root -p``` and enter your password.
5. Run ```source db/schema.sql``` from the `E-Commerce-Back-End` directory. 

## Usage Guide

1. Open a terminal instance in the `E-Commerce-Back-End` directory.
2. Call ```node server.js```
3. While the server is running, the api will accept http requests on its api route.
    - ```.../api/categories/``` - display and interact with category related data
        - ```/``` accepts get and post requests. 
        - ```/:id``` accepts get, put, and delete requests. 
        - post and put require a "category_name" key in the body of the request.
    - ```.../api/products/``` - display and interact with product related data
        - ```/``` accepts get and post requests. 
        - ```/:id``` accepts get, put, and delete requests. 
        - post and put require a "product_name", "price", "stock", and "tagIds" keys in the body of the request.
    - ```.../api/tags/``` - display and interact with tag related data
        - ```/``` accepts get and post requests. 
        - ```/:id``` accepts get, put, and delete requests.
        - post and put require a "tag_name" key in the body of the request.

## Tutorial Video

[Click here for tutorial video]()