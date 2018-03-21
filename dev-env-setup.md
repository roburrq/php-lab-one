### Dev Environment Setup

The purpose of this guide is to setup the local development environment for our server side module of this course.

To be able run our server side applications (`PHP` as the server side language and `MySQL` as the database), we need a local [Web Server](https://en.wikipedia.org/wiki/Web_server) to run our PHP applications.

There are several options for us to achieve this, but for this course we will use the option **2** below

1. [PHP Built-in web server ](http://php.net/manual/en/features.commandline.webserver.php)

      - To use the built-in web server use command `php -S localhost:8000`
        
        from the root of your application `public folder`
        
      - or `php -S localhost:8000 -t `/full/path/to/webapp/public/folder`

2. [Download MAMP](https://www.mamp.info/en/downloads/) (__**Recommended**__) - It works on both Windows and Mac operating systems.

   Once installed you will have **PHP**, **MySQL** and **PhpMyAdmin** ready for use on your machine.
   
   __**NOTE:**__ You can go to [MAMP for Mac](http://documentation.mamp.info/en/MAMP-Mac/) or [MAMP for Windows]   (http://documentation.mamp.info/en/MAMP-Windows/) for full documentation.

   Step 1 - Install the downloaded MAMP
        
   Step 2 - Launch MAMP and click `Start Servers`, you should see Apache and MySQL Servers running as seen below
        
   ![Alt text](./mamp_gui_on.png "Servers on")
   
   __**Note to Windows users**__
   
    - When you click `Start Servers` you may get a prompt that **port 80 is already in use**,

      if that happens click on `use next free port`, it will display the next port to use `e.g port 81`.
      
      If you didn't get any prompt as described above, your port is **80**.
      
    - In any case, take note of the port and anywhere you see **8888** in the rest of this guide replace it with your own port 
    
      as seen above.
      
   Step 3 - Click `Open WebStart page` to open the start page of your local web server.
      
   Step 4 - Visit http://localhost:8888/MAMP/index.php?page=phpinfo&language=English and you should see `phpinfo` page
        
   Step 5 - Visit http://localhost:8888/MAMP/index.php?page=phpmyadmin&language=English to see `phpmyadmin`
                
      from there you can manage your MySQL databases
                
   Step 6 - Now we can add our first web app powered by PHP.
        
      - On Mac, the web server is serving sites from the directory - `/Applications/MAMP/htdocs/`,
       
      - On Windows the location is `C:\MAMP\htdocs\`

      - Go ahead and create your new application folder - `mywebapp` inside the `htdocs` folder.

      - Create a PHP file - `index.php` inside the created folder `mywebapp`

      - Put the code below inside your `index.php`

      ```php
            <?php
               echo "Welcome to my PHP App!"; // You can put anything message inside the quote
      ```
      
      - Visit `http://localhost:8888/mywebapp` and 
      
        you should see `Welcome to my PHP App!` printed on the browser.
      
      - You are set, see you in class!
