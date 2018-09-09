# Udacity-Linux-Server

This is the final project of the Udacity Full Stack Nanodegree program. This is a linux server setup to run on port 80 as a web server hosting the item catalog project done earlier in the nanodegree.

The IP address of the server is 52.207.52.169

The URL to access is 52.207.52.169.xip.io

The following is a list of software that was installed to get the server running correctly: SQLAlchemy, Flask, Oauth2Client, and Python.

The server is configured to allow ssh connection through port 2200 only, as well as allowing an http connection through port 80, and an ntp connection through port 123. It is setup to deny all other connections through both the UFW firewall, and through the Amazon Lightsail Instance manager.

Third Party resources include both Google for the login ability and xip.io for the domain resolving.
