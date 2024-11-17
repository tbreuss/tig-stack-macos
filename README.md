# TIG Stack on macOS

This repository uses docker-compose (Docker must be pre-installed on your machine) to set up a local Telegraf, InfluxDB and Grafana stack (known as TIG stack).

You can use this repository to collect system data with Telegraf, store it in InfluxDB and create diagrams in Grafana.

## Installation

Copy `.env.dist` to `.env`:

```
$ cp .env.dist .env
```

Change the parameters in `.env` with the ones you like:

```
$ vi .env
```

Start the application in the background:

```
$ make start
```

Or start the application in the foreground:

```
$ make start-dev
```

Open Grafana web application <http://localhost:3000> and login with the credentials you setup in the `.env` file.

Stop the application:

```
$ make stop
```

## Uninstall

Go into the project folder and run:

```
$ make remove
```

## Thanks to

- [Han Xiao](https://github.com/justlaputa/collectd-influxdb-grafana-docker)
- [Cristian Perez Brokate](https://github.com/cristianpb/collectd-influxdb-grafana-docker)
- [Claudio Proietti](https://github.com/H4M1O/mamo)
- [Kamalashree Nagaraj](https://medium.com/@nagaraj.kamalashree/b989b2faf9f8)
