# Flask Boilerplate 4Geeks Academy

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://github.com/jwalters221/flask-rest-api)

## How to stat the project?

There is an example API working with an example database. All your application code should be written inside the `./src/` folder.

- src/main.py (it's were your endpoints should be coded)
- src/mode.py (your database tables and serialization logic)
- src/utils.py (some reusable classes and functions)

For a more detailed explanation look for the tutorial inside the `docs` folder.

## Remember migrate every time you change your models

You have to migreate and upgrade the migrations for every update your make to your models:
```
$ pipenv run migrate (to make the migrations)
$ pipenv run upgrade  (to update your databse with the migrations)
```


## Instalation for ubuntu
1. Make sure you have python 3.6+
```sh
$ pipenv install (to install pip packages)
$ pipenv run migrate (to create the database)
$ pipenv run start (to start the flask webserver)
```
ASSIGNMENT
Sample E-Commerce Site

1. Add 3 fields to Person Model:
    -first_name
    -last_name
    -phone
2. Update your main.py file to accommodate new fields through API
3. Add 3 People to Person table through SQLite3
4. Add 3 People to Person table through API
5. Create new Model Cart:
    -id (Auto Incrementing ID)
    -person_id
    -create_date
6. Create new Model CartItem:
    -id (Auto Incrementing ID)
    -cart_id
    -product_id
    -quantity
    -price
7. Create new Model Product
    -id (Auto Incrementing ID)
    -description
8. Populate your Products table with at least 3 products
9. Build new API endpoints:
    -/cart POST=create new cart and add item to cart through 1 request
    -/cart/[cart_id] GET=get cart contents from cart id (include product descriptions)
    -/cart/[cart_id]/[cart_item_id] PUT=update cart contents of 1 line item
    -/cart/[cart_id]/ DELETE=delete cart based on cart ID

    **Bonus** IMPLEMENT ANY OTHER API ENDPOINTS THAT MAY BE USEFUL?