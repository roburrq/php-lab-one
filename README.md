### Dev Environment Setup

The purpose of this guide is to setup the local development environment for our server side module of this course.

To be able run our server side applications (`PHP` as the server side language and `MySQL` as the database), we need a local [Web Server](https://en.wikipedia.org/wiki/Web_server) to run our PHP applications.

We have several options to achieve this:

#### Local dev

* [PHP Built-in web server ](http://php.net/manual/en/features.commandline.webserver.php)

        - To run the built-in web server run `php -S localhost:8000` from the root of your application `public folder` or `php -S localhost:8000 -t `/full/path/to/application/public/folder`

* [Download MAMP](https://www.mamp.info/en/downloads/) - It works on both Windows and Mac operating systems.


#### Production

* [Nginx](https://nginx.org/en/)

* [Apache HTTP Server](https://httpd.apache.org/)
