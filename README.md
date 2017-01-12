# docker-node-red
Node-Red on Alpine Linux

## Run container
```bash
docker run -d \
    --name nodered \
    -v ~/data/nodered:/data \
    -p 1880:1880 \
    0dittyspace/node-red
```
## Custom run
Run node-red to another port
```bash
docker run -d \
    --name nodered \
    -v ~/data/nodered:/data \
    -e PORT=80 \
    -p 80:80 \
    0dittyspace/node-red
```
