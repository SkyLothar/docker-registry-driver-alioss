# Docker registry alioss driver

This is a [docker-registry backend driver](https://github.com/dotcloud/docker-registry/tree/master/depends/docker-registry-core) based on the [AliOss](http://www.aliyun.com/product/oss/) key-value storage.

[![PyPI version][pypi-image]][pypi-url]
[![Build Status][travis-image]][travis-url]
# [![Coverage Status](https://coveralls.io/repos/noxiouz/docker-registry-driver-elliptics/badge.png?branch=master)](https://coveralls.io/r/noxiouz/docker-registry-driver-elliptics?branch=master)
## Usage

Assuming you have a working docker-registry and an alioss account.

`pip install docker-registry-driver-alioss`

Edit your configuration so that `storage` reads `alioss`.


## Options

You may add any of the following to your main docker-registry configuration to further configure it.

```yaml
storage: alioss
alioss_datacenter: ""
alioss_logfile: "/tmp/docker-registry-alioss.log"
alioss_loglevel: debug
```

## Developer setup

Clone this.

Get your python ready:
You are ready to hack.
In order to verify what you did is ok, just run `tox`.

This will run the tests provided by [`docker-registry-core`](https://github.com/dotcloud/docker-registry/tree/master/depends/docker-registry-core)


## License

This is licensed under the Apache license.
Most of the code here comes from docker-registry, under an Apache license as well.

[pypi-url]: https://pypi.python.org/pypi/docker-registry-driver-elliptics
[pypi-image]: https://badge.fury.io/py/docker-registry-driver-elliptics.svg

[travis-url]: http://travis-ci.org/noxiouz/docker-registry-driver-elliptics
[travis-image]: https://secure.travis-ci.org/noxiouz/docker-registry-driver-elliptics.png?branch=master
