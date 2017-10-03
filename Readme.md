# Ansible Puppet Agent Role

Install and minimally configure puppet-agent.

## how to use 

1. Create your inventory file under inventories/
1. Make sure at least one of the two variables that configure resolving puppet master is defined.
    * `pa_master_addr`
    * `pa_master_fqdn`
1. Run
    ```
    ansible-playbook -i inventories/yourinventory agent.playbook.yml
    ```
You will find an example of inventory file in the directory. 

### hiera

This module does not update the the hiera file and the site.pp. 

You need to do it in git. 
