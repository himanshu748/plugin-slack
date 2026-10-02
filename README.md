# Slack Trigger example validation

Local Kestra 2.0.2 editor screenshots and exact annotation YAML for plugin-slack issue #33. The examples use secret placeholders; the local server used dummy fixtures. No live Slack events were sent.

| Example | Before | After |
| --- | --- | --- |
| App mentions | [Missing required key](example-2-before.png) | [Valid flow](example-2-after.png) |
| New messages | [Existing conditions error](example-1-before.png) | [Conditions error remains](example-1-after.png) |

The app-mention example validates after adding the key. The new-messages example retains an unsupported `conditions` field under Kestra 2.0.2; that separate defect remains outside the required-key contribution.

The before and after YAML files preserve each complete example. These are local validation results, not evidence of a live Slack integration.
