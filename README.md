# [nexe-playground](https://github.com/jaredallard/nexe)

Learn and experiment with [nexe](https://github.com/jaredallard/nexe)

nexe lets you *create a single executable out of your node.js apps*

## Install

```sh
$ npm install nexe -g
```

## Running

There are two methods to run nexe, command line and by specifying the paramaters in `package.json`

### Command line

```sh
$ nexe -r 4.2.4 -i ./index.js -o ./main.nex
```

> Downloads node source 4.2.4 for the platform it's running on in `./tmp` directory, compiles
> it, uses browserify on `./index.js` then bundles it all an outputs `./main.nex`

### `package.json`

`nexe` property of `package.json` specifies all the parameters

```sh
$ nexe

# output is ./main.nex, which is specified in the nexe.output property
```
