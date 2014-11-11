# Busybox-Ubuntu

An extension to the original [busybox ubuntu](https://registry.hub.docker.com/_/busybox/) image with a bunch of goodies:

* a `default` non root user as recommended by [Docker's best practices](http://docs.docker.com/articles/dockerfile_best-practices/#user)
* `curl` with ssl support (no certificats installed however)
* `gosu` to run the unprivileged commands

The resulting image is slightly bigger than the original one as `curl` weights almost 10MB but you can safely delete it after user if you need a smaller image.
