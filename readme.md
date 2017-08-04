# ViCo - Count website viewers in real time with TCP!

## What is ViCo?
**ViCo** is a plugin in PHP that enables a webadmin gather statistics in real-time about their visitors. 

## How it works!
By using TCP sockets in PHP, it is built to send set data to a listening server and parse that information and keep track of the count of users entering the site all at once and in real time. 

## How to use/deploy it!
You need, of course, a website capable of running PHP 7.0+, and a listening server that will keep track of logs and such.

#### Add to page you want to track:
```php
<?php
include 'counter.php'; // File including the Class/Object

$vico = new ViCo(); // Initiate new instance of class ViCo.
$vico->ViewCounter('localhost', 9000); // Connect to server, port, and start logging
?>
```

#### Run this on you're listening server
```bash
blackvikingpro@localhost:~$ chmod +x counter.py
blackvikingpro@localhost:~$ ./counter.py &
```
This will start listening for all connections coming from the page you are tracking! Run this first!

***

## TODO
* Add more identifying information in data bundle to listening server about the client
* Implement listener in multiple language
* Add live listener onto website, using Node.JS

## Thanks for the support!
Hey thanks so much for checking this out for me! I really hope you guys enjoy it and find it useful. Please support me by following me on social media!
* Twitter: [@BlackVikingPro](https://twitter.com/BlackVikingPro)
* GitHub: [@BlackVikingPro](https://github.com/BlackVikingPro)
    * GitHub Gist: [@BlackVikingPro](https://gist.github.com/BlackVikingPro)
* Snapchat: [@blackvikingpr0](https://www.snapchat.com/add/blackvikingpr0)
* My Website: [Cygbyte Blog](https://www.blackvikingpro.xyz/)