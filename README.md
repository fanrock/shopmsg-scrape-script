ShopMessage Assignment for creating Scraping Script
==========================================
Implement a node.js based Shopify store product scraper. The goal of this project is to find information about all the products on a given site (https://www.puravidabracelets.com). 

Results should be outputted in a .csv file.
Columns:
  - product_id
  - product_title
  - variant_id
  - variant_title
  - inventory_quantity
  - captured_timestamp

We should be able to invoke your program through something like:
```
$> node scrapeInventory.js --site www.puravidabracelets.com --file outfile.csv
```

Resources
---------
You should leverage these two endpoints:

Products Endpoint:
`[shopify site domain]/products.json`
i.e.
`https://www.puravidabracelets.com/products.json` 

Paginate with `page` param


Product Details Endpoint
`[shopify site domain]/products/[handle].json`
i.e.
`https://www.puravidabracelets.com/products/sunset-surf-session-anklet.json` 


To get a better understanding of products/variants: https://help.shopify.com/en/themes/customization/products 

Deliverables
------------
**Code** - Upload your code to your own personal github account and send us a link to your completed implementation when finished.

**Deployment** - _optional_ If you have an account, upload your build to [Heroku](https://www.heroku.com/) or similar cloud hosting provider and send us a link. There is a [free tier](https://www.heroku.com/pricing#heroku-dyno-free) available so you should not have to pay. Make sure to set your `NODE_ENV=production` environment variable in the production environment. 

**Screencast** - Our team really values communication! Please make a screencast where you show us the functionality you implemented. This can be quick (no more than 5 minutes) and casual. If you don't have a tool you currently use to make screencasts, we recommend you use [Loom](https://www.useloom.com/) to make the screencast. It's free and easy to use.
