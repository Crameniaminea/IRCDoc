Corbin Osman

Guy Verrier

ETR 164

2/20/2018

IRC Server Documentation

For this project, our goal is to set up an IRC server and have control /
moderation over it. There weren’t any rules that we had to follow, just
that we should be able to connect to this server from another system,
and not the same computer.

My major objectives for this project were as follows. I first wanted to
conduct more research and find out what I needed in order to set up the
server. This would let me know if I needed anything else for this
project. I also wanted to learn how to moderate and monitor the server
to have a bit of fun with it! After my research, I started the server
creation process, which all consisted of commands. My final step would
be to modify the server properties, customizing the server to make it
more enjoyable for users.

The first step I performed was installing the server. This was done with
the simple command of “sudo apt-get install inspircd.” This command
created the server and produced a configuration file. My next step was
to edit a few of the lines inside of this file to make the server my
own. To access the configuration file, I entered the command “sudo vim
/etc/inspircd/inspircd.conf”. This opened the file where I could edit
the settings to my preference.

The first thing I changed was the server details. Below is what I
followed to do this.

![image of code](https://github.com/Crameniaminea/IRCDoc/blob/master/server.PNG)

The following is what I changed in the configuration file.

&lt;server name=”\*server.dragonroost.com\*” description=”\*Home of the
Dragons!\*” network=”\*DragonNet\*” id=”\*00D\*”&gt;

The only thing I needed to change here that was necessary was the server
name, as this is what a user enters to connect to my server. The
description is to tell a user what the server is about.

The next thing I changed was the admin details. I followed the following
to do this.

![image of code](https://github.com/Crameniaminea/IRCDoc/blob/master/Admin.PNG)

Here is what I entered into the configuration line.

&lt;admin name=”\*Crameniaminea\*” nick=”\*Dragomenia\*”
email=<*dragomenia@gmail.com*>&gt;

I configured this part of the file to create a user who had control over
the server. If I ever wanted to rule over the other dragons, I would
sign into this account (With the password I set later) as an operator.

The last thing I changed was the server address, which is where the
server would be located. Below is what I followed in order to make this
change.

![image of code](https://github.com/Crameniaminea/IRCDoc/blob/master/address.PNG)

The following is what I changed the address with.

&lt;bind address=”\*111.111.111.111\*” port=”6667” type=”clients”&gt;

164.106.166.121 is the IP address is for the computer I am using, which
is where the server is located. If this is set incorrectly, then no one
would be able to connect.

I really only learned one thing throughout the process of creating my
IRC server. That is that not entering the correct information will most
likely ruin the whole process. This means someone trying to connect to
the server must enter the right server name or they will not be able to
connect. I experienced this when first trying to connect to my own
server, which did not work for me because I did not use a pound sign in
front of the name.

In conclusion, the process of creating the server was fairly
straightforward. The only problems I encountered where when I tried
connecting to my server, which was only due to incorrect information I
entered. I really enjoyed this project and will definitely use this in
the future with friends.

Work Cited

https://samuelhewitt.com/blog/2016-04-09-how-to-deploy-an-irc-server-on-ubuntu
