# Onion-Website
How to craete onion website by android

if  you want to create your own DarkWeb site you should know this important things. To create your my own onion site you don't need buy any hosting and domain name.
Its totally hosted through your computer thats mean whenever you want you can close your site or run your site.
Note if your computer is shutdown than automatically your site will stop.

# Follow the step :-

* **Install Termux app and open a new terminal and follow the command below.**

```
$apt update 
$apt upgrade
```

* **To install tor follow the command**

```
$pkg install tor
```

# How to change tor configuration file

* **After install the tor you need to some change on tor configuration file**

```
$cd
$pkg install nano
$cd ..
$cd usr/etc/tor
$nano torrc
```

* **scroll down and this message remove the hash tag before the HiddenserviceDir and set you path.**


```
## Once you have configured a hidden service, you can look at the
## contents of the file ".../hidden_service/hostname" for the address
## to tell people.
##
## HiddenServicePort x y:z says to redirect requests on port x to the
## address y:z.

HiddenServiceDir /data/data/com.termux/files/home
HiddenServicePort 80 127.0.0.1:8080

#HiddenServiceDir /data/data/com.termux/files/usr/var/lib/tor/other_hidden_service/
#HiddenServicePort 80 127.0.0.1:80
#HiddenServicePort 22 127.0.0.1:22

################ This section is just for relays #####################
```

```
type your keyboard Ctrl+x 
y 
now enter key to save the file
```

* **To run a local server on your phone you need to install php server for that type the command.**

```
$cd
$nano index.html
```

* **Create your own script or if you want you can copy and paste my script**

```
<!DOCTYPE html>
<html>
<body>
<br>
<center>
<img height="100" width="100" src=/dark.png />
<p class="Download" > <i><b>DarkWeb</b></i></P>
<h1 style="color: blue;"> Subscribe my Channel</h1>
</center>
<style>
body {
background-color: black;
}
.Download {
border: none;
color: red;
padding: 12px 30px;
font-size: 100px;
}
</style>
</body>
</html>
```
And save it

* **open a new terminal and type the command**

```
pkg install php
php -S 127.0.0.1:8080
```


