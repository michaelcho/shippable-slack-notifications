Shippable --> Slack Notifications
=============================

This is a simple script to post notifications to a Slack channel after a build on Shippable has finished.

### Setup
- Add the deploy/notify_slack.sh file in your application. Read the comments in the file if there are any permission issues.
- Update your shippable.yml file to include the `after_success` and `after_failure` sections *especially making sure to replace the slack webhook URL with your own*. You can ignore / replace the rest of shippable.yml with whatever you are using.

### Other Configuration
- Shippable has a list of [common environment variable](http://shippable-docs-20.readthedocs.org/en/latest/config.html#common-environment-variables) which you can use in your slack message
- You get your Slack webhook URL by going to https://your-team.slack.com.services/new (replace with your team URL obviously) and setting up a new Incoming Webhook. You should get a URL that looks like https://hooks.slack.com/services/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

