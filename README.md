# SellerApp-Amazon-Project

This is the project which scrapes the data from amazon and store it in database.

Install the following before running this code :

Docker : docker.com/products/docker-desktop
Postman : postman.com/downloads/


Ports Used :
8080 : Scraper API
8081 : Collector API
27017 : Mongo DB

Scraper API (POST 8080) :
Scraper API takes POST request with url of the amazon website as data and writes the required information in mongo DB database.

Collector API (GET 8081):
Collector API takes GET request and read the product details present in mongo DB database.


Follow the following commands to run this code :

1. docker-compose build
2. docker-compose up -d

To close the service run : 
docker-compose down