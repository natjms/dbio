# dbio - Share your bio via the InterPlanetary File System

dbio is a web application that allows you to very easily publish an [about.me](https://about.me)-style web page to IPFS.

## Using
To use this app, your node needs to be writable with CORS enabled. You can do
that by running:

```
$ ipfs config --json Gateway.Writable true
$ ipfs config --json API.HTTPHeaders.Access-Control-Allow-Origin '["*"]'
$ ipfs config --json API.HTTPHeaders.Access-Control-Allow-Methods '["PUT", "POST", "GET"]'
```

## Running

First, like all good Node.JS projects, you've got to run:

```
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

All the files are accessed using relative links, so you can host the entire app on your IPFS node by pinning the `www` directory, or you can host it wherever you like.
