### Dev Environment Setup

The purpose of this guide is to setup the local development environment for our server side module of this course.

To be able run our server side applications (`PHP` as the server side language and `MySQL` as the database), we need a local [Web Server](https://en.wikipedia.org/wiki/Web_server) to run our PHP applications.

There are several options for us to achieve this:

#### Local dev

1. [PHP Built-in web server ](http://php.net/manual/en/features.commandline.webserver.php)

        - To run the built-in web server use `php -S localhost:8000`
        
          from the root of your application `public folder`
        
        - or `php -S localhost:8000 -t `/full/path/to/webapp/public/folder`

2. [Download MAMP](https://www.mamp.info/en/downloads/) (Recommended) - It works on both Windows and Mac operating systems and 
        
   and once installed you will have PHP, MySQL and PhpMyAdmin ready on your machine.
   
   *NOTE:* You can go to [MAMP for Mac](http://documentation.mamp.info/en/MAMP-Mac/) or [MAMP for Windows](http://documentation.mamp.info/en/MAMP-Windows/) for full documentation.

   Step 1 - Install the downloaded MAMP
        
   Step 2 - Launch MAMP and click `Start Servers`, you should see Apache and MySQL Servers running as seen below
        
   ![Alt text](./mamp_gui_on.png "Servers on")
      
   Step 3 - Click `Open WebStart page` to open the start page of your local web server.
      
   Step 4 - Visit http://localhost:8888/MAMP/index.php?page=phpinfo&language=English and you should see `phpinfo` page
        
   Step 5 - Visit http://localhost:8888/MAMP/index.php?page=phpmyadmin&language=English to see `phpmyadmin`
                
      from there you can manage your MySQL databases
               
   Step 6 - Visit http://localhost:8888/ - you should see `Index of /`, of course it's empty because we don't have any      
                
      site yet.
                
   Step 7 - Now we can add our first web app powered by PHP.
        
      - On Mac, the web server is serving sites from the directory - `/Applications/MAMP/htdocs/`,
       
        for Windows the location is `C:\MAMP\htdocs\`

      - Go ahead and create your new application directory `/Applications/MAMP/htdocs/mywebapp`

      - Create a PHP file inside the created directory `/Applications/MAMP/htdocs/mywebapp/index.php`

      - Put the code below inside your `index.php`

      ```php
            <?php
               echo "Welcome you my PHP App!"; // You can put anything message inside the quote
      ```
      
      - Visit `http://localhost:8888/mywebapp` and you should see `Welcome you my PHP App` printed on the browser.
      
      - You are set - See you in class.


#### Production

For production deployment, we can use any of the web servers below:

1. [Nginx](https://nginx.org/en/)

2. [Apache HTTP Server](https://httpd.apache.org/)
