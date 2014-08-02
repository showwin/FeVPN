FeVPN
=====

This is a **VPN Auto Connection** native app for Mac.  
FeVPN means **Forever VPN**.  
Download: [http://www.showwin.asia/contents/FeVPN/FeVPN.zip](http://www.showwin.asia/contents/FeVPN/FeVPN.zip)


## How FeVPN Works
Every 15 seconds, FeVPN check a condition of VPN.  
At that time, if the connection is broken, FeVPN try to reconnect VPN.  
FeVPN notifies you like this:  
![notification](http://www.showwin.asia/contents/FeVPN/FeVPN_notification.png)

## How to use
Download app from [http://www.showwin.asia/contents/FeVPN/FeVPN.zip](http://www.showwin.asia/contents/FeVPN/FeVPN.zip).

**Before opening FeVPN, you have to set VPN which you want to use.**

1. Open "Network" of "System Preferences".  
![11](http://www.showwin.asia/contents/FeVPN/FeVPN_11.png)

2. Click "Set Service Order...".  
![12](http://www.showwin.asia/contents/FeVPN/FeVPN_12.png)

3. Confirm that the VPN which you want to use has a higher priority than other VPNs.  
![13](http://www.showwin.asia/contents/FeVPN/FeVPN_13.png)

4. Settings Finished.

**Now you can open FeVPN, this app immediately starts connecting VPN.**



## Hide FeVPN
If you don't want to see icon on the dock, like this:  
![21](http://www.showwin.asia/contents/FeVPN/FeVPN_21.png)
![22](http://www.showwin.asia/contents/FeVPN/FeVPN_22.png)

**You can hide FeVPN as following steps:**

1. Right click on FeVPN and choose "Show Package Contents".
![23](http://www.showwin.asia/contents/FeVPN/FeVPN_23.png)

2. Open `/Contents/Info.plist` with Xcode.
![24](http://www.showwin.asia/contents/FeVPN/FeVPN_24.png)

3. Select "Editor" → "Add Item" on menubar.
![25](http://www.showwin.asia/contents/FeVPN/FeVPN_25.png)

4. Add highlighted line.  
(choose "Application is ..." as key and value is "YES".)
![26](http://www.showwin.asia/contents/FeVPN/FeVPN_26.png)

5. Restart FeVPN.

6. When you want to quit FeVPN, please type this command in Terminal app.
```
$ kill -9 `ps -ax | grep [F]eVPN | awk '{print $1}'`
```

## Licence
Copyright (c) 2014 Shogo ITO.  
Released under the [MIT](http://opensource.org/licenses/mit-license.php) license.

