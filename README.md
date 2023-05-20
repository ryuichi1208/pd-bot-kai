# pd-bot-kai
It is a bot that enables easy handling of PagerDuty operations from Slack, written in Go. You can also easily create your own endpoints.

## Features

* It displays details of the on-call schedule for the past 24 hours.
* Override the on-call schedule.
* Display the recent on-call schedule.

## Installation

#### Run locally

``` sh
$ export SLACK_TOKEN=xxxxxxxxxxxx
$ export PAGERDUTY_TOKEN=xxxxxxxxxxxx
$ docker-compose up
```

#### Run Kubernetes

```
$ kubectl apply -f manifests/
```
