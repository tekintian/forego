## forego

<a href="https://circleci.com/gh/ddollar/forego">
  <img align="right" src="https://circleci.com/gh/ddollar/forego.svg?style=svg">
</a>

[Foreman](https://github.com/ddollar/foreman) in Go.

### Installation

[Downloads](https://dl.equinox.io/ddollar/forego/stable)

##### Compile from Source

    $ go get -u github.com/tekintian/forego
    cd github.com/tekintian/forego
    make

    more info? [please read this article go语言Linx编译打包步骤](https://github.com/tekintian/docker-gen/blob/master/docs/compile-step-by-step.md)

### Usage

    $ cat Procfile
    web: bin/web start -p $PORT
    worker: bin/worker queue=FOO

    $ forego start
    web    | listening on port 5000
    worker | listening to queue FOO

Use `forego help` to get a list of available commands, and `forego help
<command>` for more detailed help on a specific command.

### License

Apache 2.0 &copy; 2015 David Dollar
