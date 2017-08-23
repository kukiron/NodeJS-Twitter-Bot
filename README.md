# Node.js Twitter Bot

This bot returns 10 tweets for a specified search query then favorites each of the returned tweets.

## How to use
* To use it clone this repo & install the only dependency.
```
> git clone https://github.com/kukiron/NodeJs-Twitter-Bot.git
> npm install
```
* Open <code>config.js</code> and change its values - this file will store the configuration details for the Twitter API.
```
module.exports = {
  consumer_key: '',
  consumer_secret: '',
  access_token_key: '',
  access_token_secret: ''
}
```
* Visit the [Twitter API](https://apps.twitter.com/app/new) and fill out the form to get your Keys and Access Token.
* In <code>app.js</code> edit the <code>params</code> variable to determine what to search for:
```
var params = {
  q: 'SEARCH_QUERY_HERE', //search query
  count: 10, //number of tweets to return
  result_type: 'recent', //shows recent tweets
  lang: 'en' //language English
}
```
* Now open up the command prompt and type <code>npm start</code> to run the application.
