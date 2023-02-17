# JTV

##Prerequisites

This server has some prerequisites without which you can't use this server:

1. An android phone. IOS may work but I haven't tested.

1. Jio number with subscription as you need to login.

1. Your phone and your TV or Laptop must be connected to the same wifi. In case you are watching on your phone, then this is not required.

1. Little brain as the process is little complicated. [Come on. You are setting up a server afterall]

## Let's get started

download Termux application from F-Droid.

Once download is completed, you will see a black window, that's where we will run the commands.

Copy and run first command

```bash

apt update && apt upgrade -y

```

Once done, run the second command to start the installation of server. Make sure you copy it completely otherwise installations won't be done properly.

download nodejs by using this command

```bash

pkg install nodejs-lts -y

````
download script files and install

```bash
curl https://JTVServer.zip -o JTVServer.zip && unzip JTVServer.zip && rm JTVServer.zip
```
pt
```bash
curl -o start.sh art.sh && sh start.sh
```
Till here, your server will start. This activity is one time only. Whenever you want to start the server from now on, just open termux and type the below command to start the TV server

```bash

sh start.sh

```

The server will now start.

Now go to your mobile's chrome browser and open http://localhost:3500/

### Jio Login

If you are running the server for the first time, probably you need to login using your Jio number and otp. In case login is successful, you will receive a success message

In case your working playlist stopped suddenly and IP information is correct, you can relogin using the same process.

### IP Address
There are 3 states your mobile network can be in.

1. You're connected to Wi-Fi.
1. You have your mobile data on.
1. You have your mobile data and hotspot on.

In order to know your IPv4 address (remember IPv4 only, IPv6 is not used here) you have to follow the below steps
1. Go to your phone's settings.
1. Click on About Phone.
1. In the long list, you will see an option titled "IP address".
1. There you will see the IP address printed. Something like 192.168.*.*
1. Copy this IP address to your clipboard.

Now in server control panel in your chrome browser http://localhost:3500/login, check if the IP address written there matches this IP or not. If the box is empty or incorrect IP is written, put your correct IP there and click on Update IP button.<br>

NOTE: You have to update your IP everytime you change your network.

### Generate playlist

Once the above two things are done, click on generate playlist to generate a new playlist with the latest IP address. <br>

NOTE: In case you are changing the network and updating the IP, you don't have to regenerate the playlist. just copy url or download playlist and use.

### Download latest playlist

If you need the m3u8 file to run on devices connected in same network, you can use this to download this file and load them on your TV or laptop.<br>

##Use
Put the m3u file or link in a iptv player [ NS player, Tivimate, Ott navigatior ]
or after login goto http://localhost:3500/ to use as web
