# tc-webrtc-signaling


- /config/*, package.json, server.js, sockets.js, test.js were copied from [https://github.com/andyet/signalmaster](https://github.com/andyet/signalmaster) (v0.2.2)
- You need to mount your .pem file to /src/certssl/site.pem in container. See example of a docker run:

`
docker run -ti -d --name webrtc-signaling -v /path/to/your/pem/file.pem:/src/certssl/site.pem -p 8888:8888 voduytuan/tc-webrtc-signaling
`
