# My First Express Application

This is my first Express.js application. It sets up a simple server that responds with "Hello World!!" when accessed at the root URL (`/`).

## Code

```javascript
import express from "express";
const app = express();
const port = 5000;

app.get('/', (req, res) => {
  res.send("Hello World!!");
});

app.listen(port, () => {
  console.log(`Server running on port ${port}.`);
});
