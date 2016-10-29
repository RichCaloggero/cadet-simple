# Simple Skeleton for Cadet Without Need for Node Backend

## What This Is

A very simple demonstration of how one can manage a single block of data via pouchDB / couchDB without a node backend.
We have operations new, load, save, and delete.
The data is stored in an object called cadet.
All you need do now is add your data to the object and let the database do the heavy lifting.

PouchDB can interface with a number of non-sql databases, but CouchDB is simple, and open source.
PouchDB can alternatively run just in the browser, which will be much faster and not require the CouchDB executable to be installed and running. It has adapters for IndexDB and WebSQL, the two main browser-based database engines.  THus, we should be able to use one codebase to run on most major browsers.




## Setting up pouch and couch

Follow instructions at 
https://pouchdb.com/getting-started.html

## Set up CORS
CORS is a web technology that allows web sites to use resources from another domain. You will want to enable this in your CouchDB before continuing, because otherwise PouchDB will not work unless it's served from exactly the same domain as CouchDB.

Enabling CORS is easy. Just install this handy script:
$ npm install -g add-cors-to-couchdb
And run it:
$ add-cors-to-couchdb

## Setup Caddy

A very simple web server; executables for all major platforms.  See instructions here:
https://caddyserver.com/docs/getting-started

## Run Caddy

From the command line, change to the folder where you placed these files and run caddy, changing the address found in Caddyfile if desired.
Once its running, visit the address in your browser (preconfigured as localhost:3000/cadet.html ) and your good to go.

