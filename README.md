# Go-ERD [WIP]

Entity Relationship Diagrams for Golang with GraphViz. This fork of the Go-ERD package supports multiple packages (though that support is somewhat buggy).

# Why

Visualize package's types and their inter-relationships to aid exploring and studying source code.

# Installation

```
go get github.com/lelandbatey/go-erd
```

# Use

```
# go-erd -path <path> [-path <path>]...
# ie
go-erd -path $(go env GOROOT)/src/image -path $(go env GOROOT)/src/image/color |dot -Tsvg > /tmp/out.svg
open out.svg
```

### go/ast

![go/ast](https://cdn.rawgit.com/gmarik/go-erd/master/examples/go-ast.svg)

### go/types

![go/ast](https://cdn.rawgit.com/gmarik/go-erd/master/examples/go-types.svg)

### net/http

Simple on the outside very complex on the inside.

![go/ast](https://cdn.rawgit.com/gmarik/go-erd/master/examples/net-http.svg)
