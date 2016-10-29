# Setting up pouch and couch

Follow instructions at 
https://pouchdb.com/getting-started.html

## Set up CORS
CORS is a web technology that allows web sites to use resources from another domain. You will want to enable this in your CouchDB before continuing, because otherwise PouchDB will not work unless it's served from exactly the same domain as CouchDB.

With this installed, you do not need a web server to run...

Enabling CORS is easy. Just install this handy script:
$ npm install -g add-cors-to-couchdb
And run it:
$ add-cors-to-couchdb
