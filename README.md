FeVPN
=====

This is a **VPN Auto Connection** native app for Mac.  
If your VPN is not connected, FeVPN try to connect automatically every 15-sec.  

# Download
Check releases [HERE](https://github.com/showwin/FeVPN/releases) and please download `FeVPN.zip`.

# How FeVPN Works
Every 15 seconds, FeVPN check a condition of VPN.  
At that time, if the connection is broken, FeVPN try to reconnect VPN.  
FeVPN notifies you like this:  
![notification](https://github.com/showwin/FeVPN/blob/master/images/notification.png)

# How to use
Download `FeVPN.zip` from [HERE](https://github.com/showwin/FeVPN/releases).

**Before starting FeVPN, you have to set up VPN service.**

1. Open "Network" of "System Preferences".  
![step1](https://github.com/showwin/FeVPN/blob/master/images/step1.png)

2. Click "Set Service Order...".  
![step2](https://github.com/showwin/FeVPN/blob/master/images/step2.png)

3. Confirm that the VPN service which you want to use has a higher priority than other VPN services.  
![step3](https://github.com/showwin/FeVPN/blob/master/images/step3.png)

4. Settings Finished.

**Now you can open FeVPN, this app immediately starts connecting VPN.**



## Quit FeVPN
```
$ kill -9 `ps -ax | grep "[F]eVPN" | awk '{print $1}'`
```

## Licence
Copyright (c) 2014 Shogo ITO.  
Released under the [MIT](http://opensource.org/licenses/mit-license.php) license.
