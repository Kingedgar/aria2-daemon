Aria2 daemon
---
Only 23Mb. Inspired by XUJINKAI.  

### Install
I. replace **/DOWNLOAD_DIR** and **/CONFIG_DIR** for save data, and **YOUR_SECRET_CODE** for security. Run command below  
```
sudo docker run -d \
--name aria2-daemon \
-p 6800:6800 \
-v /CONFIG_DIR:/conf \
-v /DOWNLOAD_DIR:=/download \
-e SECRET=YOUR_SECRET_CODE \
-e PGID=1002 \
-e PUID=1000 \
kingedgar/aria2-daemon:latest
```

### Build:  
`sudo docker build -f Dockerfile -t kingedgar/aria2-daemon:latest`  

### Link:  
https://github.com/aria2/aria2  
