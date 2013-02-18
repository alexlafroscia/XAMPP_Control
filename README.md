#XAMPP Control

An Alfred workflow for controlling XAMPP

***

##Commands

XAMPP control does three basic things; check whether the process is running, start the process, or stop it.  You can either check the status of `apache` or `mysql` independently, or check them both together through the `xampp` command.

Below are the basic commands available.  I will give the examples with the `xampp` command, but you can substitute it for `apache` or `mysql` if you want to turn them on and off indivudually

###Checking Status

If you're not sure if the processes are running, you can check simply by typing

    xampp

into Alfred.  It will produce a notification telling you the status of either apache, mySQL, or the both of them.

###Turning processes on or off

If you want to turn the processes on, a simple

    xampp on

will do the trick.  If you want to turn them off, the command would be

    xampp off

Really riviting stuff here, folks.

***

##Installation

There is little you have to do, other than double clicking the workflow, to get it to install.  However, in order to prevent XAMPP from asking for your administrator password every time, you can automate that bit by providing it to the Applescripts have make XAMPP Control work.

To get this working, install XAMPP Control and open up each of the Apple Script parts of the workflow, of which there are three.  Near the top of each, there are variables for `username` and `password`; set these to the name and password of an administrator on your computer, and the commands will be run with their permissions automatically.  I'm sure I don't have to tell you that this does pose a security risk should someone see them there, but I'll mention it anyway.

Also, the Applscripts assume that XAMPP has been installed in the default location (the /Applications folder for your computer).  If this is not the case, please modify the Applescripts accordingly.

*Note: If anyone knows of a way to not store those values in plaintext but still access them through Applescript, please drop me a line.*

***
##Future Plans

At some point, I may add controls for FTP through XAMPP as well, but it's not a priority since it's not something that I ever make use of.  It wouldn't be accessable through the main `xampp` command, but I may make it one of the seperate ones, like `apache` or `mysql`.

***

Anyway, thanks for checking out my first real Alfred workflow.  It's simple, but actually really handy.  It's one less app you have to deal with, at least.

