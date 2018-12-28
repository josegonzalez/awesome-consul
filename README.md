# Awesome Consul [![Build Status](https://api.travis-ci.org/josegonzalez/awesome-consul.svg?branch=master )](https://travis-ci.org/josegonzalez/awesome-consul)

This is a list of awesome third-party consul projects, libraries.

## Why consul

+ Easy to install
+ HTTP APIs
+ Design for distributed system
+ Flexible health check
+ Excellent documentation

## Table Of Contents

- Projects
    - [Alerting](#alerting)
    - [Authentication and Authorization](#authentication-and-authorization)
    - [Backup and Restore](#backup-and-restore)
    - [CLI Tools](#cli-tools)
    - [Command Execution](#command-execution)
    - [Configuration Management](#configuration-management)
    - [Monitoring](#monitoring)
    - [Other](#other)
    - [Packaging](#packaging)
    - [Provisioning](#provisioning)
    - [Programming Language Clients](#programming-language-clients)
    - [Service Discovery](#service-discovery)
    - [Errata](#errata)
- Links
    - [Articles](#articles)
    - [Presentations](#presentations)

## Projects

### Alerting

+ [consulalerting: Alert groups, teams, individuals by tags and plugins](https://github.com/jrxFive/consulalerting)
+ [consul-alerts: Simple daemon to send notifications based on Consul health checks](https://github.com/AcalephStorage/consul-alerts)

### Authentication And Authorization

+ [consult: Consul helper tool for quick query based SSH and more](https://github.com/outbrain/consult)
+ [ssh-hecate: SSH authorized_keys management via Consul](https://github.com/ncfritz/ssh-hecate)

### Backup and Restore

> *As of Consul 0.7.1, you can use [consul snapshot](https://www.consul.io/docs/commands/snapshot.html) for some use-cases.*

+ [Consul KV backup](https://github.com/kailunshi/consul-backup)
+ [consul-backinator](https://github.com/myENA/consul-backinator)
+ [consul-snapshot: A consul backup daemon to S3](https://github.com/pshima/consul-snapshot)

### CLI Tools

+ [consul-cli: Command line interface](https://github.com/mantl/consul-cli)
+ [consul-bash-completion: Consul Bash Completion library](https://github.com/nzroller/consul-bash-completion)

### Command Execution

> *As of Consul 0.5, you can use [consul lock](https://www.consul.io/docs/commands/lock.html) for many of these tasks.*

+ [cdsh: Distributed SSH](https://github.com/grubernaut/cdsh)
+ [consul-do: Do something based on leadership status](https://github.com/zeroXten/consul-do)
+ [consul-lock: Runs another program with a Consul session/kv locked.](https://github.com/fujiwara/consul-lock)
+ [consul-locker: Enforce that a program runs only on one machine at a time in a datacenter.](https://github.com/fidian/consul-locker)
+ [cronsul: Very simple distributed periodic job scheduler](https://github.com/EvanKrall/cronsul)
+ [dkron: Distributed, fault tolerant job scheduling system](http://dkron.io/)
+ [metronome: Scheduling tool on Consul](https://github.com/cloudconductor/metronome)
+ [sifter: Helps to prevent Consul from firing prematurely](https://github.com/darron/sifter)

### Configuration Management

+ [confd: Manage local application configuration files using templates and data from etcd or consul](https://github.com/kelseyhightower/confd)
+ [consul-template: Generic template rendering and notifications with Consul](https://github.com/hashicorp/consul-template)
+ [crypt: Store and retrieve encrypted configs](https://github.com/xordataexchange/crypt)
+ [envconsul: Read and set environmental variables for processes from Consul](https://github.com/hashicorp/envconsul)
+ [hashi-helper: Disaster Recovery and Configuration Management for Consul and Vault](https://github.com/seatgeek/hashi-helper)
+ [hiera-consul: Hiera backend plugin for Consul](https://github.com/lynxman/hiera-consul)
+ [kvexpress: Go program to move data in and out of Consul's KV store](https://github.com/DataDog/kvexpress)
+ [Consul.conf: responsive web interface for managing configuration of your services in Consul KV store](https://github.com/lukaszlach/consul-conf)

### Load Balancing

+ [consul-envoy: Consul to Envoy Bridge](https://github.com/jippi/consul-envoy)
+ [fabio: A fast, modern, zero-conf load balancing HTTP(S) router for deploying microservices managed by consul](https://github.com/fabiolb/fabio)
+ [Træfɪk: a modern reverse proxy](https://traefik.io/)
+ [nginx-upsync-module - Nginx C module, sync upstreams from consul or others](https://github.com/weibocom/nginx-upsync-module)

### Monitoring

+ [liaison: A daemon that collects service health information from Consul and converts it to time series data](https://github.com/cruatta/liaison)

### Other

+ [consul-topology-visualizer: Visualize latency between your Consul nodes](https://github.com/vmarchaud/consul-topology-visualizer)
+ [consulfs: ConsulFS is a FUSE distributed filesystem backed by a Consul Key-Value store](https://github.com/bwester/consulfs)
+ [git2consul: Mirrors for multiple git repos](https://github.com/breser/git2consul)
+ [uwsgi-consul: uWSGI plugin for consul integration](https://github.com/unbit/uwsgi-consul)

### Packaging

+ Debian
    + [bcandrea/consul-deb](https://github.com/bcandrea/consul-deb)
+ RPM
    + [tomhillable/consul-rpm](https://github.com/tomhillable/consul-rpm)

### Provisioning

+ Ansible
    + [griggheo/ansible-consul-template](https://github.com/griggheo/ansible-consul-template)
    + [mattupstate/vpc-consul](https://github.com/mattupstate/vpc-consul)
    + [savagegus/ansible-consul](https://github.com/savagegus/ansible-consul)
    + [sgargan/consul](https://github.com/sgargan/consul)
+ Chef
    + [adamkrone/chef-consul-template](https://github.com/adamkrone/chef-consul-template)
    + [darron/consul-cookbook](https://github.com/darron/consul-cookbook)
    + [johnbellone/consul-cookbook](https://github.com/johnbellone/consul-cookbook)
+ Docker
    + [hashicorp/docker-consul](https://github.com/hashicorp/docker-consul)
    + [foostan/consul-with-docker](https://github.com/foostan/consul-with-docker)
    + [gliderlabs/docker-consul](https://github.com/gliderlabs/docker-consul)
+ Puppet
    + [solarkennedy/puppet-consul](https://github.com/solarkennedy/puppet-consul)
+ Salt
    + [systembell/salt-consul](https://github.com/systembell/salt-consul)

### Programming Language Clients

+ Go
    + [armon/consul-api](https://github.com/armon/consul-api)
    + [consulstructure: Decode Consul data into Go (Golang) structures and watch for updates](https://github.com/mitchellh/consulstructure)
+ Java
    + [Ecwid/consul-api](https://github.com/Ecwid/consul-api)
    + [OrbitzWorldwide/consul-client](https://github.com/OrbitzWorldwide/consul-client)
+ Node.js
    + [gjohnson/consul-node](https://github.com/gjohnson/consul-node)
    + [silas/node-consul](https://github.com/silas/node-consul)
+ PHP
    + [baldurrensch/consul-php](https://github.com/baldurrensch/consul-php)
    + [sensiolabs/consul-php-sdk](https://github.com/sensiolabs/consul-php-sdk)
+ Python
    + [cablehead/python-consul](https://github.com/cablehead/python-consul)
    + [gmr/consulate](https://github.com/gmr/consulate)
    + [xav-b/pyconsul](https://github.com/xav-b/pyconsul)
+ Ruby
    + [WeAreFarmGeek/diplomat](https://github.com/WeAreFarmGeek/diplomat)
    + [xaviershay/consul-client](https://github.com/xaviershay/consul-client)
+ Scala
    + [codacy/scala-consul](https://github.com/codacy/scala-consul)

### Service Discovery

+ [connectable: Magic proxy for internal services](https://github.com/gliderlabs/connectable)
+ [registrator: Service registry bridge for Docker with pluggable adapters](https://github.com/gliderlabs/registrator)
+ [resolvable: Host-level DNS gateway for Docker](https://github.com/gliderlabs/resolvable)

## Links

### Articles

+ [Consul at Datadog](https://www.datadoghq.com/blog/engineering/consul-at-datadog/ ) - Article by Darron Froese on how Datadog deploys consul in production.
+ [Consul for Cluster Health Monitoring](https://www.vividcortex.com/blog/2015/05/22/consul-for-cluster-health-monitoring/) - Owen Zanzal writes about using Consul in place of nagios for cluster monitoring.
+ [Monitoring Consul Health and Performance](https://www.datadoghq.com/blog/monitor-consul-health-and-performance-with-datadog/) - Article by @vagelim on how to monitor consul.
+ [Securing Consul](https://www.mauras.ch/securing-consul.html) - Article on making your consul setup more secure than the defaults give you.
+ [Managing Secrets with Vault and Consul](https://testdriven.io/managing-secrets-with-vault-and-consul) - This post looks at how to set up and use Hashicorp's Vault and Consul to securely store and manage secrets.

### Presentations

+ [Running Consul at Scale—Journey from RFC to Production](https://www.usenix.org/conference/srecon16/program/presentation/froese) (SRECON 2016)

### Errata

#### ZeroRPC

[consul.d](consul.d) is an example configure file that consul working with ZeroRPC.

First, start a zerorpc server:

```
$ zerorpc --server --bind tcp://*:8081 time
```

Then, start the consul agent and the web UI:

```
$ bin/consul agent -config-dir ./consul.d
```
