# console-ticker
Un programa simple que emite un 'tick' en la consola cada 5 segundos, útil para propósitos de demostración y pruebas de tiempo.

Comandos permitidos
```
npm install
npm run test
npm start
```

# Comandos importantes usados aquí

## BUILDX
[Buildx Referencia](https://docs.docker.com/build/building/multi-platform/#getting-started)
```
# docker buildx build --platform linux/amd64,linux/arm64,linux/arm/v7 \
#    -t klerith/cron-ticker:latest --push .

# /app /usr /lib
# FROM --platform=linux/amd64 node:19.2-alpine3.16
# FROM node:19.2-alpine3.16
FROM --platform=$BUILDPLATFORM node:19.2-alpine3.16
```