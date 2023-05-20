# pd-bot-kai
It is a bot that enables easy handling of PagerDuty operations from Slack, written in Go. You can also easily create your own endpoints.

## Features

The following features have been implemented to perform operations from within Slack.

* Display the on-call summary.
* Put the specified service into maintenance mode.
* It displays details of the on-call schedule for the past 24 hours.
* Override the on-call schedule.
* Display the recent on-call schedule.

When viewing [the PagerDuty API reference](https://developer.pagerduty.com/api-reference/), you will find many other features available. However, this Bot currently implements only a subset of those features. Additional functionalities will be implemented gradually in the future as needed.

## Installation

Note: Each requires both read and write permissions.

#### Run locally

``` sh
$ export SLACK_TOKEN=xxxxxxxxxxxx
$ export PAGERDUTY_TOKEN=xxxxxxxxxxxx
$ docker-compose up
```

#### Run Kubernetes

Please update the manifests to include the respective tokens.

```
$ kubectl apply -f manifests/
```
