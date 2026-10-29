# Axle Wrapper for glfw library

> Original repository: [glfw/glfw](https://github.com/glfw/glfw)

This repository is *only* a wrapper for release of glfw library. No code was written by author of this repository.

Created especially for [axle](https://github.com/agnostic-t/axle) build system.

## Before using

This repo contains pre-build script, that builds glfw from sources, therefore install build dependencies beforehand.

## How to use

In order to use this module, in your `module.json`:

```json
{
  "remote_deps": {
    "glfw3": {
      "version": ">=0.0.0",
      "url": "https://github.com/agnostic-t/wrap-glfw3"
    }
  },
}
```

In dependencies of modules:

```json
{
  "dependencies": {
    "glfw3": { "version": ">=0.0.0" }
  }
}
```

Before running, if you compiled dynamic version set LD_LIBRARY_PATH:

```sh
export LD_LIBRARY_PATH=./.vendor/glfw3/.modules/glfw3/bin
```
