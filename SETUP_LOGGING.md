# Setup Logging
taken from the [nodejs setup](https://devcenter.heroku.com/articles/getting-started-with-nodejs#introduction) documentation
```
git clone https://github.com/heroku/node-js-getting-started.git
cd node-js-getting-started
heroku create
heroku ps:scale web=1
git push heroku master
heroku open
heroku addons:create papertrail
heroku addons:open papertrail
heroku addons:create flydata:feather
heroku addons:create logentries:le_tryit
heroku addons:open logentries
heroku addons:open flydata
heroku ps:scale web=0
```
