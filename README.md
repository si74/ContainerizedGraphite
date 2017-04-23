# ContainerizedGraphite
graphite + carbon + whisper & collectd

This repository, however, contains a docker-compose file for collectd and statsd. To use the docker-compose file,
simply run `docker-compose up`.

Docker-compose file uses the following images:

(1) collectd

[Collectd](https://hub.docker.com/r/andreasjansson/collectd-write-graphite/)

I personally git cloned the collectd repo, built my own image, re-tagged it, and used that in the docker-compose file. Note that you will need to replace the placeholder in the docker compose file with your image name.

(2) graphite + carbon + whisper

I got lazy and decided to use this docker image for the actual graphite + paraphernalia part.

[Docker-Graphite](https://github.com/nickstenning/docker-graphite)
