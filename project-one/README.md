# Test Project One

Layout is to enable both running from commandline via ansible-playbook commands, as well as supporting running from ansible tower.

The root of the execution folder is ./playbooks/

The inventory files are very small, and contain the minimum neccessary to be valid.

the group_vars directory is where all playbook variables are stored (in directories that map to inventory groups)

## runme.yml

This playbook allows full running and variable substitution by using just the selected inventory file

## rungroup.yml

This playbook requires an additional parameter to be passed at runtime (the appropriate inventory groupname).  This allows for a check to ensure the runner is in the correct environment.
