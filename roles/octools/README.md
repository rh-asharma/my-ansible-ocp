octools
=========

This role use oc tools to communicate with the openshift master

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

---
projectname: test
template: nodejs-example
apphostname: mynodejsapp
templatename: phptemplate
createtemplate: false
quickapp: false
sti: false
git_url: https://github.com/dudash/openshift-workshops.git
url_to_template: https://github.com/dudash/openshift-workshops.git
scaleme: false
autoscale: false
username: laurent
pass: redhat
contextdir: .
number_of_instances: 1
ochost: https://osemaster.rdu.salab.redhat.com
ocport: 8443
appdomain: apps.rdu.salab.redhat.com

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

GPLv2

Author Information
------------------

This role was created in 2016 by Laurent Domb
