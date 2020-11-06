# go-swf

[![GoDoc](https://godoc.org/github.com/wojciechbator/swf?status.svg)](https://godoc.org/github.com/wojciechbator/swf)
[![Build
Status](https://travis-ci.org/wojciechbator/swf.svg?branch=master)](https://travis-ci.org/wojciechbator/swf)
[![Go Report Card](https://goreportcard.com/badge/github.com/wojciechbator/swf)](https://goreportcard.com/report/github.com/wojciechbator/swf)
[![Go Coverage](http://gocover.io/_badge/github.com/wojciechbator/swf)](https://gocover.io/github.com/wojciechbator/swf)

Package swf contains utilities to read Shockwave Flash Format files.
Originally created by Kelvyne - github.com/Kelvyne/swf, it was refactored
to use Go modules and the errors in Reader were fixed as the old project
is not maintained.

### Documentation

See [here](https://godoc.org/github.com/wojciechbator/go-swf)

### Example

```go
parser := swf.NewParser(r)
swfFile, err := parser.Parse()
fmt.Printf("Tags count : %v\n", len(swfFile.Tags))
```
