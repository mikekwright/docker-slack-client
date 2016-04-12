Docker Slack Client
=========================================================================

This is a simple client, the one thing it requires is that you send it an environment variable that has the token
for you to use to connect to slack.  

## Examples

        # This will send the default 'Hello World' message by the bot owner of the token to the channel #general
        docker run --rm -e SLACK_TOKEN=<mytoken> mikewright/slack-client

        # This will send the message "Hi there" to channel "#my-channel"
        docker run --rm -e SLACK_TOKE=<mytoken> -e SLACK_CHANNEL=#my-channel mikewright/slack-client "Hi there"

