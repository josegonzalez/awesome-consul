
This is a list of awesome third-party consul projects, libraries.

## Why consul

+ Easy to install
+ HTTP APIs
+ Design for distributed system
+ Flexible health check
+ Excellent documentation

## Awesome consul

+ [Package](#Package)
+ [Provision](#provision)
+ [Programming Language Clients](#programming-language-clients)
+ [Notification](#notification)
+ [Practices](#practices)


### Package

+ Debian
    + [bcandrea/consul-deb](https://github.com/bcandrea/consul-deb)
+ RPM
    + [tomhillable/consul-rpm](https://github.com/tomhillable/consul-rpm)

### Provision

+ Docker
    + [progrium/docker-consul](https://github.com/progrium/docker-consul)
    + [foostan/consul-with-docker](https://github.com/foostan/consul-with-docker)
+ Puppet
    + [solarkennedy/puppet-consul](https://github.com/solarkennedy/puppet-consul)
+ Salt
    + [pravka/salt-consul](https://github.com/pravka/salt-consul)
+ Ansible
    + [sgargan/consul](https://github.com/sgargan/consul)
    + [jivesoftware/ansible-consul](https://github.com/jivesoftware/ansible-consul)
    + [mattupstate/vpc-consul](https://github.com/mattupstate/vpc-consul)
    + [griggheo/ansible-consul-template](https://github.com/griggheo/ansible-consul-template)
+ Chef
    + [johnbellone/consul-cookbook](https://github.com/johnbellone/consul-cookbook)
    + [adamkrone/chef-consul-template](https://github.com/adamkrone/chef-consul-template)
    + [darron/consul-cookbook](https://github.com/darron/consul-cookbook)


### Programming Language Clients

+ PHP
    + [baldurrensch/consul-php](https://github.com/baldurrensch/consul-php)
    + [sensiolabs/consul-php-sdk](https://github.com/sensiolabs/consul-php-sdk)
+ Go
    + [armon/consul-api](https://github.com/armon/consul-api)
+ Java
    + [Ecwid/consul-api](https://github.com/Ecwid/consul-api)
    + [OrbitzWorldwide/consul-client](https://github.com/OrbitzWorldwide/consul-client)
+ Node.js
    + [gjohnson/consul-node](https://github.com/gjohnson/consul-node)
    + [silas/node-consul](https://github.com/silas/node-consul)
+ Python
    + [cablehead/python-consul](https://github.com/cablehead/python-consul)
    + [gmr/consulate](https://github.com/gmr/consulate)
    + [hackliff/pyconsul](https://github.com/hackliff/pyconsul)
+ Ruby
    + [WeAreFarmGeek/diplomat](https://github.com/WeAreFarmGeek/diplomat)
    + [xaviershay/consul-client](https://github.com/xaviershay/consul-client)
+ Scala
    + [codacy/scala-consul](https://github.com/codacy/scala-consul)

### Notification

+ [consul-alerts](https://github.com/AcalephStorage/consul-alerts)

### Practices

#### Configure Management

+ [confd](https://github.com/kelseyhightower/confd)

#### Service Discovery

[consul.d](consul.d) is an example configure file that consul working with ZeroRPC.

First, start a zerorpc server:

```
$ zerorpc --server --bind tcp://*:8081 time
```

Then, start the consul agent and the web UI:

```
$ bin/consul agent -config-dir ./consul.d
```

#### Others

+ [Consul KV backup](https://github.com/kailunshi/consul-backup)
+ [Mirrors for multiple git repos](https://github.com/Cimpress-MCP/git2consul)
+ [Do something based on leadership status](https://github.com/zeroXten/consul-do)
+ [uWSGI plugin for consul integration](https://github.com/unbit/uwsgi-consul)
+ [Command line interface](https://github.com/CiscoCloud/consul-cli)
+ [Store and retrieve encrypted configs](https://github.com/xordataexchange/crypt)
