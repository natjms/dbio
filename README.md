# dbio - Share your bio via the InterPlanetary File System

dbio is a web application that allows you to very easily publish an [about.me](https://about.me)-style web page to IPFS.

## Running the app

First, like all good Node.JS projects, you've got to run:

````
$ npm install
```

Since this project was started a long time ago, it uses Elm 0.18.0. Binaries for this version aren't available using NPM anymore. Instead, this version of Elm must be downloaded as a tarball from a github repository. To do this, run:

```
$ npm run install-tarballs
```

Now, you can use

```
$ npm run build
$ npm start
```
