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
