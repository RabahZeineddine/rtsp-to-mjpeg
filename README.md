# rtsp-to-mjpeg

Simple container to provide access to a RTSP stream via MJPEG.

The image requires the following environment variables to be set:

CAMERAUSER=''\
CAMERAPASSWORD=''\
CAMERAIP=''\
CAMERAPORT=''\
CAMERASTREAM=''

## Docker

```bash
docker container run --rm -e CAMERAUSER='' -e CAMERAPASSWORD='' -e CAMERAIP='' -e CAMERAPORT= -e CAMERASTREAM='' -p 9000:8080  rabahzein/rtsp-to-mjpeg
```

## Docker-Compose

```yml
version: "2"
services:
  rtsp-to-mjpeg:
    image: rabahzein/rtsp-to-mjpeg
    environment:
      - CAMERAUSER=
      - CAMERAPASSWORD=
      - CAMERAIP=
      - CAMERAPORT=
      - CAMERASTREAM=
    ports:
      - 9000:8080
```
