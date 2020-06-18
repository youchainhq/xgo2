# xgo2 - Go CGO cross compiler

fork from:

https://github.com/gythialy/xgo

which fork from:

https://github.com/karalabe/xgo

using Docker Hub to hold the images

# enhanced

## --goproxy

enable `GOPROXY` environment variable when compiling

## --envlist

Send more environment variables when compiling.

An example is to set the `GOPRIVATE` when a go mod project references some private modules (and in this case the `GOPROXY` should be a custom one).

```shell
xgo2 --envlist="GOPRIVATE=private.git.repo.com"
```

# install

```go
go get -u github.com/youchainhq/xgo2
```
