# Build process

## Requirements

- git
- nodejs 10.x
- yarn
- npm

### Notes

#### Devuan

`yarn` is known as `yarnpkg`.

## Building lw.comm-server

```
> git clone -b windows-build https://github.com/trombik/lw.comm-server.git
> cd lw.comm-server
> yarn --frozen-lockfile
> yarn prep
> yarn build
```

## Running lw.comm-server

```console
> nodejs ./server.js
```

## What `yarn build` does

The repository has a sub-module, `LaserWeb4`. It builds `LaserWeb4` by running
`npm run bundle-dev` in the sub-module directory, which creates an asset.  The
asset is copied to `app` directory. See `scripts` in `package.json`.
