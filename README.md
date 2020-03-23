<img src="ssftps.svg" width=128>
# Stupidly Simple FTP Server

## What is it?
This python script is based on Giampaolo Rodola's pyftplib Library and aims to
bring this program to anybody whithout the need for a command line nor python knowledge.
It is written on top of the GTK3 Toolkit running consequently on any major distro.

## Requisites:
On any ubuntu-ish distro, you may install the library with the following command line:
```
sudo apt install python3-pyftpdlib
```

## How does it work?
When you open the program, you are presented with this screen:
![](Interface_1.png)

If you just click the switch, the server will start with it's default values:
![](Interface_3.png)

These values are:

* Port: 2121
* User: anonymous
* Pass: none
* Dir : . (that is the local directory the program is run from)

The anonymous user has no write permissions though. This may be fine with you, but if you want to be able to explore your filesystem, upload and change files, you have to add a user. To accomplish this, just push the config button prior to starting the server:

![](Interface_2.png)

Go ahead and change the values to suit you needs. The values are stored, as soon as the dialog is closed, so no apply or save procedure is neccessary. Now go ahead and flick the switch and enjoy the server...

## Known Issues
Setting the loglevel to anything higher than INFO as well as getting an ERROR,
causes the program to crash with a segfault. I will have to look into that more closely.

## Based on
`pyftplib` library by Giampaolo Rodola

`pyGObject` library 