# Bookstore Payment Confirmation using STRIPE API
To use this feature you need to register on official stripe page and get both publish and secret keys.


### package.json
  ```
    {
      ...
      "dependencies": {
        "body-parser": "^1.20.2",
        "cors": "^2.8.5",
        "dotenv": "^10.0.0",
        "express": "^4.17.1",
        "stripe": "^8.191.0"
    }
  }
  ```

After you have cloned this repo to you local machine you can install all dependencies typing in terminal
```
  npm install
```
Make sure that you are in right derictory. After that start server
```
  node server.js
```



## API instructions
- GET
    Get the publish key to setup stripe in frontend using url: "http://localhost:5252/config"
- POST
    create stripe payment intent using url: "http://localhost:5252/create-payment-intent"
    object that sends:
  ```
   {
      "amount": number
  }
