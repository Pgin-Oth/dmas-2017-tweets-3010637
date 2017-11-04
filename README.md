# DMAS 2017 Tweets project
## Student ID: 3010637
This is an Aurelia application.
App address: https://dmas-2017-tweets-3010637.herokuapp.com/index.html

To deploy this single page application into Heroku, you need to do as below:
1. Under project folder run command: "au build" .
2. Copy file "index.html" and folders "scripts" and the others we need into deployment folder. 
3. cd deployment_folder.
4. Create index.php with contents: <?php header( 'Location: /index.html' ) ;  ?>
5. Commit and push the project into heroku.
6. Take a tag of release.

Bellows are some useful commands:
  heroku git:clone -a dmas-2017-tweets-3010637
  git init
  heroku login
  heroku create
  heroku apps:create dmas-2017-tweets-3010637
  heroku logs --tail
  git remote add heroku git@heroku.com:{heroku-app-name}.git
  git status -su 
  git add .
  git commit -m "Comments"
  git push heroku master
  heroku config:set NODE_ENV="production"
  heroku config:set MONGOLAB_URI=mongodb://donationuser:donationuser@dsXXX.mlab.com:XXXX/donation
  heroku open
  heroku auth:token
