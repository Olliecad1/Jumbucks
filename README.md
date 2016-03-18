# How to setup Jumbucks gui and command line interface on linux or raspberry pi 

1. You will need to install jumbucks tar.gz file from here https://github.com/jyap808/jumbucks/archive/v1.9.tar.gz 
2. Once you have it installed go to file manager and navigate to Downloads and you will see a folder called jumbucks-1.9.tar.gz right click on it and click extract to then you will see a little box that called Extract files also you will see a little box with the name above Extrace to default it will be /home/pi/Downloads/ but we want to extract it to /home/pi/ so backspace until you see /home/pi then click extract at the bottom
3. Now were getting into the good stuff open up a terminal window and type ls (ls stands for list segments it lists all the segments in the current directory) once you have typed ls you will see a directory called jumbucks-1.9 so cd into jumbucks-1.9 (cd stands for change directory we are changing directory) now that your in jumbucks-1.9 type ls and you will see some more directorys now cd src and now you will see a bunch of c++ code now run this command make -f makefile.unix USE_UPNP=- this will take up to about an hour 
4. So after that has finished you can start creating the jumbucks.conf file so cd .. out of src and cd .. again out of jumbucks-1.9 and now you will be in the home/pi directory so cd .jumbucks and you will see a bunch of data and files now type the following commands sudo nano jumbucks.conf and press enter (nano is a text editor) so now type or copy and paste the following code
<p>#Config file for Jumbucks</p> 
<p>#Daemon and listen ON/OFF</p> 
<p>daemon=1</p>
<p>#listen=1</p>

<p>#Connection User and Password</p>
<p>rpcuser=changethisuser</p>
<p>rpcpassword=changethispassword</p>

<p>#Authorized IPs</p>
<p>rpcallowip=127.0.0.1</p>

<p>#write the location for this blockchain below if not on standard directory</p>
<p>#datadir=/home/media/USB/.jumbucks</p>

<p>#Add extra Nodes</p>
<p>#addnode=1.2.3.4</p> 

