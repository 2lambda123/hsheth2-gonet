# GoNet
[![GoDoc](https://godoc.org/github.com/hsheth2/gonet?status.svg)](https://godoc.org/github.com/hsheth2/gonet)
[![Build Status](https://travis-ci.org/hsheth2/gonet.svg?branch=master)](https://travis-ci.org/hsheth2/gonet)
[![License](http://img.shields.io/:license-MIT-blue.svg)](http://www.opensource.org/licenses/MIT)

A network stack written in Go with the CSP style. GoNet was written for research purposes, and the accompanying paper is titled [*An Implementation and Analysis of a Kernel Network Stack in Go with the CSP Style*](https://arxiv.org/abs/1603.05636).

**Warning: GoNet was built for research purposes and is neither production-ready nor under active development.** As an alternative, we would recommend looking into [google/netstack](https://github.com/google/netstack). 

## Usage
*Note: This project only works on linux machines (because of its dependency on the tap device).*

To install `GoNet`:

1. Run `go get github.com/hsheth2/gonet`
2. In the directory, run `make`. 

You can use its functionality by importing it in your own projects. See the GoDoc for documentation. 

We also included a simple demo application: a basic HTTP server. Once you have run `make` in the `GoNet` source directory, there will be an executable called `gohttp` in your Go bin. This executable will run the HTTP server, and will serve the files in whatever directory it is run in. 

Because `GoNet` runs on the tap interface, it will be accessible at `10.0.0.2`. 

## Contributors
This project was created by [Harshal Sheth](https://github.com/hsheth2)
and [Aashish Welling](https://github.com/omegablitz). 

## License
GoNet is released under the [MIT License](http://www.opensource.org/licenses/MIT).
