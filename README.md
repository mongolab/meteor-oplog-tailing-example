meteor-oplog-tailing
====================

An example Meteor app that utilizes MongoDB oplog tailing.

Original blog post for reference: [blog.mongolab.com](blog.mongolab.com)

## Set up the app
```
> meteor create app
```

Once your Meteor project is created, cd into the "app" directory and copy the repo files there.
 
## Bundle and extract the application
```
> meteor bundle app.tgz
> tar -zxvf app.tgz
```

## Create a "local" database user
If you're using MongoLab, you can visit our docs to find [instructions on creating a "local" database user](http://docs.mongolab.com/oplog/).
 
## Run the application with the command:
```
> PORT=3000 MONGO_URL=<your_uri> MONGO_OPLOG_URL=<your_local_uri> node bundle/main.js
```
