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
## Configuration:
####NAME="SCREENNAME"
NAME OF THE SCREEN INSTANCE
####USER="USER"
USER OF SCREEN PROCESS. EMPTY FOR NO SWITCH.
####DIR="/WRK/DIR"
WORKING DIRECTORY. EMPTY FOR NO SWITCH.
####EXECCOMMAND="./FILETOEXECUTE"
COMMAND TO EXECUTE
####SHUTDOWNCMD="exit"
IF EMPTY STRING "" CTRL-C WILL BE SENT.
####USER OF SCREEN PROCESS. EMPTY FOR NO SWITCH.
