# Twiml-PhoneBuzz-P2

Twiml-PhoneBuzz-P2 is a Node.js app using [Express 4](http://expressjs.com/) hosted in [Heroku](https://www.heroku.com/). This is the second phase of LendUp coding challenge. Try the app [https://twiml-phonebuzz-p2.herokuapp.com](https://twiml-phonebuzz-p2.herokuapp.com)

Enter your phone number in the App and hit Submit. Then, Twilio will call your phone number and start playing Fizz Buzz. When prompted to enter a number to listen to the engine speaking in Fizz Buzz language from 1 up until the number given.

## Dependencies

During development, Twiml-Phonebuzz-P2 used these libraries (available from npm):
  * "body-parser": "v1.18.2",
  * "express": "v4.15.2",
  * "twilio": "v3.11.0"

## Running Locally

This app is not available locally, since the Twilio call URL would not accept a localhost url.

## Using Other Twilio Account

Few changes has to be made to the code:

  * Delete the accountSid in index.js line 9 and hard code your Twilio's accountSid (Not recommended) or use process.env.TWILIO_ACCOUNT_SID if you've saved your sid in local environment variable.
  * Delete the authToken in index.js line 9 and hard code your Twilio's authToken (Not recommended) or use process.env.TWILIO_AUTH_TOKEN if you've saved your token in local environment variable.
  * Change the 'from' parameter to your Twilio account number.
  * If you host the app somewhere else, change the url in line 50 in index.js

## Note

This app uses Twilio free trial, so it will not work with a non-whitelisted phone number.
