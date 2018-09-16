# All-The-News-Thats-Fit-To-Scrape

- The following npm packages need to be installed in this order.

- npm init -y
- npm install
- npm install express
- npm install express-handlebars
- npm install mongoose
- npm install body-parser
- npm install cheerio
- npm install request
- npm install method-override
- npm install morgan
- npm install loopback-connector-mongodb --save

- To run this app on heroku do the following below.
- heroku login
- heroku addons:create mongolab


- Connect the database to heroku with the following javasctipt code
```js
- // If deployed, use the deployed database. Otherwise use the local mongoHeadlines database
var MONGODB_URI = process.env.MONGODB_URI || "mongodb://localhost/mongoHeadlines";

// Set mongoose to leverage built in JavaScript ES6 Promises
// Connect to the Mongo DB
mongoose.Promise = Promise;
mongoose.connect(MONGODB_URI);
