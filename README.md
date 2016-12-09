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

