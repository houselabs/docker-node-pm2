# docker-node-pm2
a node-pm2 environment based on alpine linux

## Run a node.js app with pm2
`docker run -d -v /data/someapp:/opt/app --name someapp houstlabs/pm2`

Default entry file is app.js, you can custom entry file by specifying `APP` env variable.

## Debuging with bash
`docker exec -it someapp bash`

## Service status
`docker exec -it someapp pm2 status`

## Logs
`docker exec -it someapp pm2 logs`
