# node-prune-test

This is a sample project for trying [node-prune](https://github.com/tj/node-prune).  
[My issue](https://github.com/tj/node-prune/issues/64) is node-prune@1.1.0 via gobinaries.com does not work fine on alpine image.

## :ok_woman: node:12.15.0

[Dockerfile_full](https://github.com/TasukuUno/node-prune-test/blob/master/Dockerfile_full)
build on node:12.14.1 

```
yarn build
```

```
  Downloading github.com/tj/node-prune@v1.1.0
  Resolved version master to v1.1.0
  Downloading binary for linux amd64
  Installing node-prune to /usr/local/bin

  Installation complete
/usr/local/bin/node-prune


         files total 332
       files removed 9
        size removed 30 kB
            duration 4ms
```

## :no_good_woman: node:12.15.0-alpine

[Dockerfile_alpine](https://github.com/TasukuUno/node-prune-test/blob/master/Dockerfile_alpine)
build on node:12.14.1-alpine 

```
yarn build_alpine
```

```
  Downloading github.com/tj/node-prune@v1.1.0
  Resolved version master to v1.1.0
  Downloading binary for linux amd64
  Installing node-prune to /usr/local/bin
  Installation complete

/usr/local/bin/node-prune
/bin/sh: node-prune: not found
```
