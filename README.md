# Consul Demo

Demo about how to ususage of consule version 0.4.1

## Install consul

Download consul [here](https://www.consul.io/downloads.html), and save it to some path, `/usr/local/bin/` for example.

In this demo i just put it in the `./bin/` folder.

## Quick Start

First, start a zerorpc server:

```
$ zerorpc --server tcp://0.0.0.0:8081 time 
```

Or, if you have a zerorpc environment in a virtualenv:

```
$ path/to/zerorpc --server tcp://0.0.0.0:8081 time
```

Then, start the consul agent and the web UI:

```
$ bin/consul agent -server -bootstrap-expect 1 -data-dir /tmp/consul -ui-dir ./web/dist -config-dir ./consul.d -client 0.0.0.0
```

