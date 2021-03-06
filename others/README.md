#flask-file-server

A flask file server with an elegant frontend for browsing, uploading and streaming files

![screenshot](https://raw.githubusercontent.com/Wildog/flask-file-server/master/screenshot.jpg)

## Build
```docker build --rm -t alhaol/flask-file-server .```

## Run
```docker run -p 8000:8000 alhaol/flask-file-server```

## Params
FS_BIND = Param for bind address, default 0.0.0.0  
FS_PORT = Param for server port, default 8000  
FS_PATH = Param for serve path, default /tmp  
FS_KEY = Param for authentication key as base64 encoded username:password, default none  

```docker run -p 8000:8000 -e FS_BIND=0.0.0.0 -e FS_PORT=8000  -e FS_PATH=$PWD -e FS_KEY=YWxoYW9sOiFlbWFuITk3Nw== alhaol/flask-file-server```

