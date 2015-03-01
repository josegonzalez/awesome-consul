
This is a list of awesome consul projects, libraries.

## Why consul

+ Easy to install
+ HTTP APIs
+ Design for distributed system
+ Flexible health check
+ Excellent documentation

## Awesome consul

+ [Provision](#provision)
+ [Programming Language Clients](#programming-language-clients)
+ [Notification](#notification)
+ [Practices](#practices)

### Provision

+ [Docker](https://github.com/progrium/docker-consul)
+ [Puppet](https://github.com/solarkennedy/puppet-consul)
+ Ansible
    + [sgargan/consul](https://github.com/sgargan/consul)
    + [jivesoftware/ansible-consul](https://github.com/jivesoftware/ansible-consul)
+ Chef
    + [johnbellone/consul-cookbook](https://github.com/johnbellone/consul-cookbook)
    + [adamkrone/chef-consul-template](https://github.com/adamkrone/chef-consul-template)
    + [darron/consul-cookbook](https://github.com/darron/consul-cookbook)


### Programming Language Clients

+ [PHP](https://github.com/baldurrensch/consul-php)
+ [Go](https://github.com/armon/consul-api)
+ Java
    + [Ecwid/consul-api](https://github.com/Ecwid/consul-api)
    + [OrbitzWorldwide/consul-client](https://github.com/OrbitzWorldwide/consul-client)
+ Node.js
    + [gjohnson/consul-node](https://github.com/gjohnson/consul-node)
    + [silas/node-consul](https://github.com/silas/node-consul)
+ [Python](https://github.com/cablehead/python-consul)
+ Ruby
    + [WeAreFarmGeek/diplomat](https://github.com/WeAreFarmGeek/diplomat)
    + [xaviershay/consul-client](https://github.com/xaviershay/consul-client)

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
