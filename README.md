This is a modification to the base [MEANjs.org](http://meanjs.org/) [Yeoman deployment](http://meanjs.org/generator.html) of the MEAN.js stack. This modification adds local token authentication capabilities as an alternative of local cookie based authentication through sessions. 

## Welcome
Welcome to Whitehall Technologies LLC's open source project adding token based local authentication to the base MEANjs.org deployment of the MEAN.js stack. Please visit our [site](http://www.whitehall.io) for more info and follow us on [Twitter](https://twitter.com/castlewhitehall) and [GitHub](https://github.com/castlewhitehall) for live updates.

## Token Authentication
Token authentication is an alternative to cookie based authentication and is has a number of benefits.

* Cross-domain / CORS: cookies + CORS don't play well across different domains. A token-based approach allows you to make AJAX calls to any server, on any domain because you use an HTTP header to transmit the user information.

* Stateless (a.k.a. Server side scalability): there is no need to keep a session store, the token is a self-contanined entity that conveys all the user information. The rest of the state lives in cookies or local storage on the client side.

* CDN: you can serve all the assets of your app from a CDN (e.g. javascript, HTML, images, etc.), and your server side is just the API.

* Decoupling: you are not tied to a particular authentication scheme. The token might be generated anywhere, hence your API can be called from anywhere with a single way of authenticating those calls.

* Mobile ready: when you start working on a native platform (iOS, Android, Windows 8, etc.) cookies are not ideal when consuming a secure API (you have to deal with cookie containers). Adopting a token-based approach simplifies this a lot.

(Taken from Alberto Pose's [article](https://auth0.com/blog/2014/01/07/angularjs-authentication-with-cookies-vs-token/))


## Credits
Inspired by and built upon the great work of [MEANjs.org](http://meanjs.org/)
The MEAN name was coined by [Valeri Karpov](http://blog.mongodb.org/post/49262866911/the-mean-stack-mongodb-expressjs-angularjs-and)

## License
(The MIT License)

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
