# cool-cats
site for project supporting cat lovers.
// importing express framework
const express = require("express");

const app = express();

// Respond with "hello world" for each request that hit our root "/"
app.get("/", function (req, res) {
 return res.send("Hello World, time to start deing");
});

// listen to port 7000 by default
app.listen(process.env.PORT || 7000, () => {
  console.log("Server is running");
});

module.exports = app;
