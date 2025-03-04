# ansible-role-sshpam-webhook
webhook for sshpam

This Ansible role "sshpams" or sends notifications to webhook on detected SSH login. It can be easily integrated into your existing playbooks.
Can easily be extended to send notifications to other services, it is just curl.


## Requirements
- `Discord webhook, slack or custom webhook endpoint`
- `curl`
- maybe `jq`

## Example playbook

```yaml
- hosts: all
  roles:
    - role: sshpam
      vars:
        slack_webhook_url: ""
        discord_webhook_url: "https://discord.com/api/webhooks/1234567"
        n8n_webhook_url: ""
        custom_webhook_url: ""
```


# TODO

* more variables for script path, message
* error stuff
* git submodule instructions
* specific ip loc instructions


# Changelog
