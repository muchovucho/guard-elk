# Lavo  MD Docker Compose

## Introduction

In this project we want to demonstrate the MD project, which lays the foundation that a detect team would need.

## Requirements

Docker requirements:

- CPU: 2
- Memory: 8GB

### Docker Daemon

Change the docker daemon:

```
{
  "metrics-addr" : "127.0.0.1:9323",
  "experimental" : true
}
```

## Install


Use Docker Compose to install this solution

```
$ docker-compose up -d
```


### Access
Urls:

| App | URL | User | Pass |
|-----|-----|------|------|
|Kibana|[http://localhost:80](http://localhost:80)| elastic | changeme |
|Grafana|[http://localhost:80](http://localhost:80)|admin |admin|
|Prometheus|[http://localhost:80](http://localhost:80)|admin |admin|
|Alertmanager|[http://localhost:80](http://localhost:80)|admin |admin|
|Jenkins|[http://localhost:80](http://localhost:80) | |

#### Jenkins
To get the pass:

```
$ docker-compose logs -f jenkins
```


