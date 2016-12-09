# php-built-in-server-manager
Simple Bash script to stop, start, restart PHP built-in web server

**usage**: `./server <command> [<hostname>:<port>]`

**Available commands**:
```
  start     Starts PHP built-in web server server on specified hostname:port, default is localhost:8080  
  stop      Stops the PHP built-in web server
  restart   Stops and Starts on previously specified hostname:port
  status    Status of the process
```

## How to Use it

This is a very basic script, you're not limitted. choose one either one of these:
 - Copy `server` script to the root of the PHP project.
 - Copy/Symlink it in one of your $PATH directories e.g. `~/bin` or `/usr/local/bin` and use it everywhere.

**Note:** On start, the script creates `server.pid` and `server.log` files in current working directory  and when stopped, it only deletes the `server.pid` and `server.log` remains there.

the `server` script can be renamed to whatever you desire. I personally prefer `pmserver`.
`.pid` and `.log` files have the same name as the script file e.g. when renaming `server` to `pmserver` there will be `pmserver.pid` and `pmserver.log` files
