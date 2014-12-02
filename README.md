# libmongoose

A library based on the MIT-licensed older version of the lightweight mongoose web server.
Please see the current [mongoose](https://github.com/cesanta/mongoose) project for the latest version of that great embeddable webserver.

I created this fork as I needed a small web server as well as a http/https client on a really tight embedded platform, so it was essential to share as much code as possible between client and server to save footprint size. Therefore I built it as a library. The older version of mongoose had all I needed (the newer has much more, [check it out](https://github.com/cesanta/mongoose)), so I decided to use the older version.  
