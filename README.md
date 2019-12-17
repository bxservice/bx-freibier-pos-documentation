This repository holds all the documentation needed to run the [Freibier POS app](https://github.com/bxservice/de.bxservice.freibierpos)

The repository has the following pdf files:
-----------
* [Technical Manual](https://github.com/bxservice/bx-freibier-pos-documentation/blob/master/TechnicalManual.pdf): this document gives a technical overview of the app, list the prerequisites and steps you need to follow before running the app, and sets some guidelines for contributions.
* [Server Configuration](https://github.com/bxservice/bx-freibier-pos-documentation/blob/master/ServerConfiguration-POS.pdf): in this document you can find all the necessary steps to configure correctly iDempiere to take advantage of the app's features (How to configure the products, pos settings, etc).
* [User Manual](https://github.com/bxservice/bx-freibier-pos-documentation/blob/master/Usermanual-POS.pdf): this is the app guide, once you've configured iDempiere you can start using the app and this manual guides you through all the steps.

** THE MANUALS SHOULD BE FOLLOWED IN THE ORDER DESCRIBED ABOVE**

The file [freibierPosDemoClientSetup.zip](https://github.com/bxservice/bx-freibier-pos-documentation/blob/master/freibierPosDemoClientSetup.zip) is a packout that contains sample data to test the app in GardenAdmin, it also has the necessary web service security records to communicate the server with the app.

# TL;DR #
To test the app quickly in GardenAdmin follow these steps:

1. Install the [FCM Notifications plugin](https://github.com/bxservice/de.bxservice.bxpos.fcm-server) in your server (if you want to use the push notifications functionality, create your own API KEY).
2. Login as GardenAdmin in iDempiere and import the [freibierPosDemoClientSetup.zip](https://github.com/bxservice/bx-freibier-pos-documentation/blob/master/freibierPosDemoClientSetup.zip) pack in.
3. Set up the data in iDempiere.
     * Create the records in the "Table" window (at least one summary and one child)
     * Configure the product categories, products and product price: check the Self-Service flag in the product category and product records, and the Sold flag in the products
     * Create a record in "POS Terminal" (only one active record per org). The   following   fields   are   ​ mandatory   for   the   POS   to   work:   Sales   Representative,   Bank   Account,  Price   List,   Warehouse,   template   B.   Partner,   template   To   Go   B.   Partner   (it   can   be   the   same   as  the template one) and Document Type. 
4. Open the app in your Android device, open the connection data settings and fill the fields with your server data.
5. Go to the initial screen and introduce the username and password. If everything was configured correctly, you are now logged into the Freibier POS.
