# oip-express

oip-express is a simple webapp boilerplate using expressjs, pug, and js-oip to build a single-page FLO webapp.

## Install
```
npm install
```

## Building
Call the babel binary directly to compile js to the lib directory:
```
./node_modules/.bin/babel src --out-dir lib
```
or, use our builtin custom package script:
```
npm run compile
```

## Running
After compiling with babel, start the webserver:
```
npm start
```

For convenience, run both commands in sequence:
```
npm run compile && npm start
```

## Contents
Currently, this repo contains the Recent tZERO DLR Records webapp found at [https://floblockchain.org/tzero/](https://floblockchain.org/tzero/). 
In the future these repos will be separated and the oip-express app will contain a simple boilerplate app retrieving an unfiltered list of the latest few OIP records.

## Configuration
Configuration is done through modifying `src/index.js` at the moment. In the future a configuration file is planned. 
```
port = 3000
oip-server = snowflake.oip.fun
```
