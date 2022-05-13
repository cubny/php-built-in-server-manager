# php-built-in-server-manager
Manage PHP built-in web server like a pro

**usage**: `./server <command> [<hostname>:<port> [router]]`

**Available commands**:
```
  start     Starts PHP built-in web server server on specified hostname:port, default is localhost:8080
            router is a PHP script to which all requests will be redirected (if used)
  stop      Stops the PHP built-in web server
  restart   Stops and Starts on previously specified hostname:port
  status    Status of the process
  log       Show the PHP built-in web server logs. Use the -f option for a live update
```

## How to Use it

This is a very basic script so you're not limitted to any specific method. I suggest one of these two:
 1. Copy `server` script to root of your PHP project.
 2. Copy/Symlink to your one of $PATH directories like `~/bin` or `/usr/local/bin` and use it everywhere.

**Note:** When starts, two files `server.pid` and `server.log` will be created in current working directory and when stopped, only `server.pid` will be deleted but `server.log` remains.

the `server` script can be renamed to whatever you like. I personally prefer `pmserver`.
`.pid` and `.log` files will have the same name as the filename e.g. when `server` renames to `pmserver` there will be `pmserver.pid` and `pmserver.log` files
