# grafana

[![Build Status](https://travis-ci.com/iroquoisorg/ansible-role-grafana.svg?branch=master)](https://travis-ci.com/iroquoisorg/ansible-role-memcached)

Ansible role for grafana

This role was prepared and tested for Ubuntu 16.04.

# Installation

`$ ansible-galaxy install iroquoisorg.grafana`

# Default settings

```
grafana_http_port: 3000
grafana_http_addr: 0.0.0.0
grafana_domain: localhost
# Set to true to automatically assign new users to the default organization (id 1). Default in grafana is true but it's unsecure
grafana_auto_assign_org: false

grafana_root_url: "%(protocol)s://%(domain)s:%(http_port)s/"

# github auth, see http://docs.grafana.org/installation/configuration/#authgithub for details
grafana_github_auth_enabled: false
grafana_github_client_id: some_id
grafana_github_client_secret: some_secret
grafana_github_allow_sign_up: true
grafana_github_team_ids: []

grafana_basic_auth_enabled: true

grafana_latest: true
grafana_beta: no

```
