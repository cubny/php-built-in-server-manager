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

This is a very basic script so you're not limitted to any specific method. I suggest one of these two:
 1. Copy `server` script to root of the PHP project.
 2. Copy/Symlink to your $PATH e.g. `~/bin` or `/usr/local/bin` and use it everywhere.

**Note:** When it starts, the script creates `server.pid` and `server.log` files in current working directory and when stopped, it deletes the `server.pid` but `server.log` remains there.

the `server` script can be renamed to whatever. I personally prefer `pmserver`.
`.pid` and `.log` files will have the same name as the filename e.g. when renaming `server` to `pmserver` there will be `pmserver.pid` and `pmserver.log` files
