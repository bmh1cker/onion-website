# onion-website
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



