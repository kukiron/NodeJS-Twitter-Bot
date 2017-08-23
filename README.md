# Node.js Twitter Bot

This bot returns 10 tweets for a specified search query then favorites each of the returned tweets. It also follows 10 users who recently had popular tweets for a specified search query.

## How to use
* To use the twitter-bot clone this repo & install the only dependency.
```
> git clone https://github.com/kukiron/NodeJs-Twitter-Bot.git
> npm install
```
* Rename the file <code>config.default.js</code> in app folder to <code>config.js</code> and then change the values in it - this file will store the configuration details for the Twitter API.
```
module.exports = {
  consumer_key: '',
  consumer_secret: '',
  access_token_key: '',
  access_token_secret: ''
}
```
* Visit the [Twitter API](https://apps.twitter.com/app/new) and fill out the form to get your Keys and Access Token.
* In <code>favorite.js</code> or <code>follow.js</code> you can edit the <code>params</code> variable to determine what to search for:
```
var params = {
  q: 'SEARCH_QUERY_HERE', //search query
  count: 10, //number of tweets to return
  result_type: 'recent', //shows recent tweets
  lang: 'en' //language English
}
```
* Now you can run the application. Open up the command prompt and type <code>node app/favorite.js</code> to see the new favorites & type <code>node app/follow.js</code> to see which new users you are following based on the specified search query.
