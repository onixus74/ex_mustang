# ex_mustang

> A simple, clueless bot (that does nothing much right now)

![Mustang](images/mustang.jpg)

ExMustang is a bot for Slack written in Elixir.

_Warning: This is a work in progress._

### Setup

Create a Slack bot user from [here](https://my.slack.com/services/new/bot). You will receive an API token you can use. Set the `SLACK_API_TOKEN` environment variable and you should be good to go.

You can run this bot as below:

```shell
export SLACK_API_TOKEN="<SLACK_API_TOKEN>"
mix run --no-halt
```

### Scheduled Notifications

#### Github Pull Requests Watcher

You can configure github token by setting `GITHUB_TOKEN`. Also, you can pass list of repos to watch by updating [config](config/config.exs#L11-L17). There are bunch of other stuffs you can configure such as schedule (which follows cron format), slack channel and thresholds.

#### Standup Reminder

The standup reminder reminds us when its standup time. Our nature is that we either forget track of time or are too lazy to remember about it :P You can configure message and other bunch of stuffs on [config](config/config.exs#L5-L9)

### Responders

```shell
mustang help - Displays help message
quote - Displays random quote
```
