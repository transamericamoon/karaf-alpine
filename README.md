# karaf alpine docker image

Karaf docker image with alpine base.  Exposing deploy and data folders for persistence

```
docker run -d -t \
  --name karaf \
  -p 1099:1099 \
  -p 8101:8101 \
  -p 44444:44444 \
  -v /host/path/deploy:/deploy \
  -v /host/path/data:/data \
  transamericamoon/karaf-alpine
```
