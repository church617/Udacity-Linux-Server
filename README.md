# Udacity-Linux-Server

This is the final project of the Udacity Full Stack Nanodegree program. This is a linux server setup to run on port 80 as a web server hosting the item catalog project done earlier in the nanodegree. This server is setup to run everything through an SQLAlchemy database, no SQLIte or PostgresQL server is running, only a SQLALchemy server, much like the original project that ran on the local machine.

The IP address of the server is 52.207.52.169

The URL to access is 52.207.52.169.xip.io

The following is a list of software that was installed to get the server running correctly: SQLAlchemy, Flask, Oauth2Client, and Python.


This server is hosted on an Amazon Lightsail instance. After logging in with the private key provided, I first created the grader user to be used by the assigned Udacity grader, then gave them sudo access by using the command usermod -aG sudo grader. After this, I then setup the firewall of the server to allow only three connections, ssh on port 2200, http on port 80, and ntp on port 123. once this was done, I then went into the sshd_config file to allow entry on port 2200 for ssh as well as disabling the ability to log into the server remotely as the root user by changing the PermitRootLogin setting to no. I then updated my server to the newest version of Ubuntu by running a do-release-upgrade command to ensure everything was up to date. I then installed Flask, Oauth2Client, and Flask using a sudo apt install command, and checked to make sure python was installed with the latest verion via the same command. Once that was done, I cloned my Item catalog repo from github after changing it so that it ran on port 80. I then used a tmux command before strting upp the application so that it would continue running even after I had exited my gitbash session. Once this was done, I then attempted to access the webpage by using appending xip.io to my servers public address. Once I was able to do so, I then made sure my Login function using Googles authentication services was working. Once that was working then the server is good to go.

Third Party resources include both Google for the login ability and xip.io for the domain resolving.
