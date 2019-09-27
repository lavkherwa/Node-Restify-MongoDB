
## How to guide

Create a Free Mongo DB cluster at Mongo Altas <br>
https://cloud.mongodb.com/

Replace the MONGODB_URI in the [config file](RestWithMongoDb/config.js) with your DB instance endpoint

Clone repository and run the application to have your customer crud working 😉

## If you're new to NodeJs refer below

- Create application discriptor file (package.json) <br>
  **command:** npm init -y
- Add dependencies to our Application <br>
  **command:** npm i restify restify-errors mongoose mongoose-timestamp
- Add Dev dependencies <br>
  **command:** npm i -D nodemon
- Delete node modules folder (In case of corrupted files) <br>
  **command:** rm -rf node_modeules

- Run the application on local machine <br>
  **command:** npm run dev (NOTE: This will run nodemon, to stop press 'control + c' on mac)
  
## Security

- To enabling security install below libraries <br>
  **command:** npm i restify-jwt-community jsonwebtoken bcryptjs
