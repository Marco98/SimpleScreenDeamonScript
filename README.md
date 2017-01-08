# SimpleScreenDeamonScript
Controls a simple deamon with GNU Screen
##Please read this before usage:
####SSDS is currently not working if you are a non root user and want to su into a diffrent user!
####Please be patient, i'll work on a solution when i have the time to do so.
## Usage:
```
./ssds {start|stop|restart|status|chown|console}
```
## Deployment:
```
wget -O ./ssds https://raw.githubusercontent.com/Marco98/SimpleScreenDeamonScript/master/ssds
chmod +x ./ssds
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
