# SimpleScreenDeamonScript
Controls a simple deamon with GNU Screen
## Usage:
```
./ssds {start|stop|restart|status|chown|console}
```
## Simple Deployment:
```
wget -O ./ssds https://raw.githubusercontent.com/Marco98/SimpleScreenDeamonScript/master/ssds
chmod +x ./ssds
```
You will also need **screen**. In the Debian/Ubuntu Repos, the package is simply called "**screen**".
## Configuration:
####Just open the script with a text editor of your choice.

**NAME="SCREENNAME"**

Name of the screen instance

**NEWUSER="USER"**

User that runs the command in the screen. Empty for current user.

**NEWUSERPASSWD=""**
If su needs the Password to SU to the NEWUSER you can enter it here.

**DIR="/WRK/DIR"**

Working directory. Empty for current directory.

**EXECCOMMAND="./FILETOEXECUTE"**

Command to execute in the screen.

**SHUTDOWNCMD="exit"**

Command to send to stop the process. Empty to send a CTRL-C.

**USEWATCHDOG="false"**

If true, the Program will simply restart after a crash or close. It will only stop after using the "stop" function.
