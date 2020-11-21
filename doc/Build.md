# Build process

## Requirements

- `nodejs` 10.x
- `npm`
- `git`

## Building `lw.comm-server`

```console
git clone -b unix https://github.com/trombik/lw.comm-server.git
cd lw.comm-server
git submodule update --init --recursive
npm ci
npm build
```
