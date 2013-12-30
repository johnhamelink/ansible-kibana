kibana ansible role
=================================================================

Setup
-----

Generate a htpasswd file (You can use an online tool if you don't have apache installed - [this one is known to work](http://www.htpasswdgenerator.net/)) and put it in `roles/kibana/files/htpasswd`.

You'll need to copy the vars/global_vars.yml.sample file and adjust the settings to how your servers are set up.

Add the `kibana` group to your ansible hosts file

Installation
------------

### Kibana:

`ansible-playbook kibana.yml`
