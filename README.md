# array-vue

> Source for http://array.vc

## Build Setup

``` bash
# install node version manager - https://github.com/creationix/nvm#installation

nvm install v8
nvm alias default v8

# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

## deploying for test / next
1. Change `assetsPublicPath` in config/index.js from `/` to `/next` under `build:` section
2. Run `npm run build`
3. FTP `index.html` & `dist/` up to the `/next` dir
4. Open http://array.vc/next in browser

## deploying for reals
1. Make sure `assetsPublicPath` in config/index.js is `/` under `build:` section
2. Run `npm run build`
3. FTP `index.html` & `dist/` up to the root directory to replace existing
4. Open http://array.vc/ in browser
