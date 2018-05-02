# Simple dockerized build pipeline for Golang-Microservices 

** Not suitable for production use! **

* The **get** container `go get`'s all dependencies of a go project in the working directory.
* The **build** container compiles a static linux ELF binary (hopefully).
* The **app** container runs the compiled binary.

No need for a local Go installation and fiddling around with `GOPATH` etc.

Just `docker-compose up`.


