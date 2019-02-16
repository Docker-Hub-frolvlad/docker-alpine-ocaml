[![Docker Stars](https://img.shields.io/docker/stars/frolvlad/alpine-ocaml.svg?style=flat-square)](https://hub.docker.com/r/frolvlad/alpine-ocaml/)
[![Docker Pulls](https://img.shields.io/docker/pulls/frolvlad/alpine-ocaml.svg?style=flat-square)](https://hub.docker.com/r/frolvlad/alpine-ocaml/)


OCaml Docker image
==================

This image is based on Alpine Linux image, which is only a 5MB image, and contains
[OCaml compiler](https://ocaml.org/).

Download size of this image is only:

[![](https://images.microbadger.com/badges/image/frolvlad/alpine-ocaml.svg)](http://microbadger.com/images/frolvlad/alpine-ocaml "Get your own image badge on microbadger.com")

Usage Example
-------------

```bash
$ echo 'print_string "Hello, World!";;' > qq.ml
$ docker run --rm -v "$(pwd):/tmp" frolvlad/alpine-ocaml ocamlopt -cclib --static /tmp/qq.ml -o /tmp/qq
```

Once you have run these commands you will have `qq` executable in your current directory and if you
execute it, you will get printed 'Hello, World!'
