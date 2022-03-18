# PHP 7.3 FPM Xdebug Docker Image

### Notes
This image should only be used to specifically run xdebug workloads.

Other php images do not include xdebug because it slows performance just by being added as a php extension.

You will need to set the `XDEBUG_REMOTE_HOST` environment variable to the IP or hostname of the machine you wish
to connect and run Xdebug with. This defaults to `host.docker.internal` which allows the host to connect
when running Docker for Mac.

### History
This repo was previously included in a [mono repo](https://github.com/favish/docker-images) and the last published
tag with that repo was `php-7.3-fpm_xdebug_1.1.0`. The CircleCI build process continues to publish versions to the same image
on [Dockerhub](https://hub.docker.com/r/favish/php-7.3-fpm-xdebug). The first tag published with this repo is `2.0.0`.