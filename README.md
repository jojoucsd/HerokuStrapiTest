# Strapi application

**To Reproduce the Bug**

yarn install / npm install

* ```heroku login ```
* ```git init```
* ```git add .```
* ```git commit -m "Initial Commit"```
* ```heroku create <appName>```
* ```heroku addons:create heroku-postgresql:hobby-dev```
* ```heroku config```
* ```heroku config:set DATABASE_USERNAME=<before :>```
* ```heroku config:set DATABASE_PASSWORD=<after :  befroe @>```
* ```heroku config:set DATABASE_HOST=<after @ before : >```
* ```heroku config:set DATABASE_PORT=5432```
* ```heroku config:set DATABASE_NAME=<after / >```
* ```git  push heroku master```

* heroku may ask you yarn install again or yarn again depends if throw errors on yarn is outdated 

* app should be runing on heroku as production with a postgress DB 

* create 1 or more than 1 entries under Article in production DB

* add a required field in local development DB under content type article 

* ```git commit -am "changes"```
* ```git push heroku master ```

heroku build should be success but heroku open will leads your to ``` heroku logs --tail ```

And similar errors shows like 

* **[2020-02-29T21:08:18.400Z] error Impossible to register the 'article' model.**

* **[2020-02-29T21:08:18.401Z] error error: column "xyz" contains null values.**



