# Challenge link
https://docs.google.com/document/d/1PoxpoaJymXmFB3iCMhGL6js-ibht7GO_DkCF2elCySU/edit#

# Shopify
A web application to track inventory for Shopify or any logistic company. Built with MongoDB, Express, Angular + Angular Material Design and Node (MEAN).

## Instructions to run locally
1. Download/Clone the repository.
2. `cd Shopify`(for Windows), 'ls Shopify`(Linux) to go into the Shopify backend directory.
3. `npm install` to install npm modules required for the backend(First make sure you have nodejs installed in your system/environment. Reference link to install nodejs "https://nodejs.org/en/download/package-manager".).
4. `cd shopify-web-app`(for Windows), 'ls shopify-web-app`(Linux) to go into the "shopify-web-app" frontend directory.
5. `npm install` to install npm modules required for the frontend.
6. (Install) and start mongodb. By default it runs on port 27017. Database name is "Shopify". The path or name can be changed from config/config.json(Reference link to install mongodb "https://www.mongodb.com/docs/manual/installation/". For your local system you can just install MongoDB Compass and start the service and check the databases using GUI.)

## Follow steps 7 & 8 to start the server and steps 9 & 10 to start the frontend.
7. `cd Shopify`(for Windows), 'ls Shopify`(Linux) to go into the Shopify backend directory.
8. To start the server use command `node app.js` or `npm start`.
9. `cd shopify-web-app`(for Windows), 'ls shopify-web-app`(Linux) to go into the "shopify-web-app" frontend directory.
10. To start the frontend  use `npm start`, this command will use port 4200.
11. View in browser at http://localhost:4200

## Features
- Item Fields: Code, Name, Category, Price, Total, Remaining/Available in stock, Added On(Date when the item was added in the inventory).
- Operations: Search, add, update, delete, restore items from the inventory.
  While deleting the user can either permanently delete the item from the inventory or just temporarily delete it leaving a deletion commment(i.e. make the item unavailable due to several reasons).
  The user has an option to restore the temporarily deleted item. The user can view the deletion comments before deleting/restoring the item.
- Trivial logical checks in item add/update/delete forms like remaining quantity should be a number and less than or equal to total available quantity etc.
- The search bar extensively searches the complete inventory and finds the matching items among any of the fields. For Ex:- The user can input date as "2021" and the relevant items will be displayed in the table that were added in the year 2021. The user can use the common search bar to search among any of the available fields.
- Added a simple pagination for better user experience.


## Future Additions
- Add Warehouse management and shipment tracking.(Need 3-4 days to completely implement basic functionalities for both)
- An option that allows the user to download the inventory as csv/xlsx.
- Graphical representation of the most sold item, revenue, etc over a period of time.
The first 2 additional features will need small to moderate changes and require 3-4 days for completion). The 3rd feature will require more input data over the period as its a graphical representation.

## Note
This code for logistics inventory web application is completely working in the local system and with a few changes in the url can be used for deployment as well. As I am new to Replit, I tried creating the account and deploy the application there but couldn't find an option for angular application. While there was an option for Reactjs and no option for angular, I had to stop with the deployment. I was unable to find any tutorials for deploying a MEAN stack application on Replit.
The application is perfectly working with all the features and several logical checks, I just need a guide or steps thats help me in deploying the MEAN application on Replit.
