# Uniswap Info

[![Lint](https://github.com/Uniswap/uniswap-info/workflows/Lint/badge.svg)](https://github.com/Uniswap/uniswap-info/actions?query=workflow%3ALint)
[![Deploy](https://github.com/Uniswap/uniswap-info/workflows/Deploy/badge.svg)](https://github.com/Uniswap/uniswap-info/actions?query=workflow%3ADeploy)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)

Analytics site for the [Uniswap Protocol](https://uniswap.org).

### To Start Development

###### Installing dependencies
```bash
yarn
```

###### Running locally
```bash
yarn start
```

###### Prepare to deploy
```shell script
1. run a oasis ethereum runtime gateway with code: https://github.com/dltswap/oasis-ssvm-runtime
2. build a graph node or docker image with code: https://github.com/dltswap/graph-node, and run postgreq, ipfs, graph-node
   with instruction. It is recommended to use docker-compose to start.
3. Run a web server, such as nginx, then expose the graph service through the web server, and bind the domain name
4. Modify the service path in src/apollo/client.js and run this app.
```

###### deploy in heroku
```bash
heroku login -i

create-react-app info-dltswap
cd info-dltswap

#copy source from other direction

git init
heroku create -b https://github.com/mars/create-react-app-buildpack.git info-dltswap
git add .
git commit -m "react-create-app on Heroku"
git push heroku master
```
