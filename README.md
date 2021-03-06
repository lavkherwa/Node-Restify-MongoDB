
## How to guide

Create a Free Mongo DB cluster at Mongo Altas <br>
https://cloud.mongodb.com/

Replace the MONGODB_URI in the [config file](RestWithMongoDb/config.js) with your DB instance endpoint

Clone repository and run the application to have your customer crud working 😉

**NOTE:** Api's are protected with authentication token, please check below on how to access the api's

## NEW - Added JWT Token authentication 

Now to access any api's you need to provide token.
- Register new user <br>
  [POST] http://localhost:3000/register
- Get **token** for registered user <br>
  [POST] http://localhost:3000/auth
- Pass below header for accessing any api's <br>
  Header: Authentication <br>
  Value: Bearer **token**




## If you're new to NodeJs refer below

- Create application discriptor file (package.json) <br>
  **command:** npm init -y
- Add dependencies to our Application <br>
  **command:** npm i restify restify-errors mongoose mongoose-timestamp
  * **restify -** For creating rest api endpoints
  * **restify-errors -** For handling http errors
  * **mongoose -** For communicating with MONGO DB
  * **mongoose-timestamp -** For adding audit trail info with records
- Add Dev dependencies <br>
  **command:** npm i -D nodemon
- Delete node modules folder (In case of corrupted files) <br>
  **command:** rm -rf node_modeules

- Run the application on local machine <br>
  **command:** npm run dev (NOTE: This will run nodemon, to stop press 'control + c' on mac)
  
## Security

- To enabling security install below libraries <br>
  **command:** npm i restify-jwt-community jsonwebtoken bcryptjs
  * **restify-jwt-community -** For protecting endpoints
  * **jsonwebtoken -** For setting up auth server and creating JWT token
  * **bcryptjs -** For password encryption/decryption of the registered user
  
References: https://www.youtube.com/watch?v=bqn-sx0v-l0
