# rh-aap-sandbox-instruqt

Artifacts to create an Ansible Automation Platform 2.5 deployment on the Instruqt platform.

This follows the pattern of 1 x Gateway, 1 x Controller, 1 x Hub, 1 x EDA Controller and an external database as discussed in the [Red Hat documentation for deploying Ansible Automation Platform](https://docs.redhat.com/en/documentation/red_hat_ansible_automation_platform/2.5/html/rpm_installation/assembly-platform-install-scenario#ref-gateway-controller-hub-ext-db)

This Track requires the following environment variables to enable deployment:

* RHN_AAP_PACKAGE_CHECKSUM - used by the prerequisites role to download the appropriate offline installer for AAP
* RHN_OFFLINE_TOKEN - the RH Portal token used to authenticate and authorise the bundle download

NOTE: If the Offline Token is not used for over 30 days, it becomes stale and a new token must be generated.

## Docs for RH Portal API

- [Getting started with Red Hat APIs
](https://access.redhat.com/articles/3626371)
- [Red Hat API Tokens
](https://access.redhat.com/management/api)
