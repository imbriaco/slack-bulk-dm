slack-bulk-dm
-------------

This is a very simple Ruby utility to send a direct message to a group of users in Slack.

## Usage

1. `git clone https://github.com/imbriaco/slack-bulk-dm`
2. Generate a Slack token using the [Test Token Generator](https://api.slack.com/docs/oauth-test-tokens).
3. Set a `$SLACK_API_TOKEN` environment variable matching the token generated in the previous step. This should look something like this: `export SLACK_API_TOKEN=<token>`.
3. Edit the `message.json` file with your message and the recipient list.
3. Run `ruby slack-bulk-dm`. This will install the required depenencies, make sure that it can find users matching the provided usernames in the message file, open an IM session to each user, and send the message.
