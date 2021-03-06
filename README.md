# YouTube Uploader Client

This is a little project for upload video from a [Nextcloud](https://nextcloud.com/) repository to [Youtube](https://www.youtube.com/)
> This is a Vue.js project

## Build Setup

### Installing dependencies
``` bash
# install via NPM
npm install
```
Or
``` bash
# install via Yarn
yarn install
```

### Executing server.
Serve with hot reload at localhost:8080
``` bash
# with NPM
npm start
```
Or
``` bash
# with Yarn
yarn start
```

### Building
Build for production with minification
``` bash
# with NPM
npm run build
```
Or
``` bash
# with Yarn
yarn run build
```

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).

## Recreate proto stup class
For recreate stup class you must have follow:
- [protobuf](https://github.com/protocolbuffers/protobuf/releases)
- [protoc](https://github.com/grpc/grpc-web/releases)
- Also you can see it: [gRPC-web](https://github.com/grpc/grpc-web)
- [gRPC](https://grpc.io/docs/tutorials/basic/web.html)
After installed it just go to source code folder an run it:
```
protoc protos/youtube-uploader.proto \
--js_out=import_style=commonjs:src/grpc \
--grpc-web_out=import_style=commonjs,mode=grpcwebtext:src/grpc
```
The result is generated on: src/grpc folder
