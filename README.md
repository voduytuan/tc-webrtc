# tc-webrtc-signaling


- `/src/config/`, `/src/package.json`, `/src/server.js`, `/src/sockets.js`, `/src/test.js` were copied from [https://github.com/andyet/signalmaster](https://github.com/andyet/signalmaster) (v0.2.2)
- By default, this image will start container of mastersignal (WebRTC Signaling Socket Server) in secure mode (https), you need to prepare PEM file and  mount your `.pem` file to `/src/certssl/site.pem` in container. See example of a docker run:

```bash
docker run -ti -d --name webrtc-signaling -v /path/to/your/pem/file.pem:/src/certssl/site.pem -p 8888:8888 voduytuan/tc-webrtc-signaling
```

- To create PEM file, you can google "How to create pem file" and follow found tutorials to get your pem file from your private key and certificate from CA.
