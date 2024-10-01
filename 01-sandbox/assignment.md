---
slug: sandbox
id: 9wn0beriyhpe
type: challenge
title: Sandbox
tabs:
- id: vuxqt46hwyd0
  title: Bastion
  type: terminal
  hostname: bastion
  workdir: /opt/ansible
- id: x3a1tz9qep0s
  title: Ansible Controller
  type: website
  url: https://aap-controller.${_SANDBOX_ID}.instruqt.io
  new_window: true
- id: pr3rf3tj20a5
  title: Ansible Hub
  type: website
  url: https://aap-hub.${_SANDBOX_ID}.instruqt.io
  new_window: true
- id: 9bmtsli4rbiq
  title: Event Driven Ansible
  type: website
  url: https://eda-controller.${_SANDBOX_ID}.instruqt.io
  new_window: true
difficulty: basic
---

Red Hat Ansible Automation Platform Sandbox
===========================================

This Sandbox environment consists of the following services:

| Host | Service Description |
| -------- | -------- |
| bastion     |  Bastion Host. Installation of the AAP and host interaction can be undertaken from here.     |
| aap-controller     |  The Ansible Automation Platform Controller. The main point of interaction with AAP   |
| aap-hub     |  The Ansible Automation Platform Hub. A single source of truth for Ansible Collections and Content  |
| eda-controller     |  The Event Driven Ansible Controller.  The orchestrator of EDA integrations with AAP Controller and other services |
| postgres     |  The database host for other services in the environment   |

The password for all the services deployed here is the same as the value in the `$_SANDBOX_ID` environment variable.

```bash,run
echo $_SANDBOX_ID
```

All relevant urls can be acquired by running this command.
```bash,run
echo https://aap-controller.${_SANDBOX_ID}.instruqt.io
echo https://aap-hub.${_SANDBOX_ID}.instruqt.io
echo https://eda-controller.${_SANDBOX_ID}.instruqt.io

echo username: admin
echo password: ${_SANDBOX_ID}
```