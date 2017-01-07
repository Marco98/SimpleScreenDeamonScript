# SimpleScreenDeamonScript
Controls a simple deamon with GNU Screen

## Usage:
```
./ssds {start|stop|restart|status|chown|console}
```
## Deployment:
```
wget -O ./osctl https://raw.githubusercontent.com/Marco98/SimpleScreenDeamonScript/master/ssds
chmod +x ./osctl
```
You will also need **screen**. In the Debian Repos, the package is just called "**screen**".
## Configuration:
####Just open the script with a text editor of your choice.
**NAME="SCREENNAME"**
Name of the screen instance
**USER="USER"**
User that runs the command in the screen. Empty for current user.
**DIR="/WRK/DIR"**
Working directory. Empty for current directory.
**EXECCOMMAND="./FILETOEXECUTE"**
Command to execute in the screen.
**SHUTDOWNCMD="exit"**
Command to send to stop the process. Empty to send a CTRL-C.
