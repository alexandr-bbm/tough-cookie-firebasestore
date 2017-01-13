# Firebase Cookie Store

tough-cookie-firebasestore is a Firebase store for tough-cookie module. See 
[tough-cookie documentation](https://github.com/goinstant/tough-cookie#constructionstore--new-memorycookiestore-rejectpublicsuffixes) for more info.

## installation

    $ npm install tough-cookie-firebasestore

## Options

  `path` file path of cookiejar.

## Usage

    var FirebaseCookieStore = require("tough-cookie-firebasestore");
    var CookieJar = require("tough-cookie").CookieJar;
    var app = firebase.initializeApp({ ... });
    var rootPath = "/cookies"
    
    var jar = new CookieJar(new FirebaseCookieStore(app, rootPath));

## License

 MIT
