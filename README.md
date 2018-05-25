# Simple dockerized build pipeline for Golang-Microservices 

## Not suitable for production use!
Use a single multistage build container for serious projects

* The **get** container `go get`'s all dependencies of a go project in the working directory.
* The **build** container compiles a static linux ELF binary (hopefully).
* The **app** container runs the compiled binary.

No need for a local Go installation and fiddling around with `GOPATH` etc.

Invoke with `docker-compose up get && docker-compose up build && docker-compose up app` or e.g. just `docker-compose build`.


