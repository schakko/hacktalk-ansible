# Hacktalk Wolfsburg - Ansible
## Part 3: Environments
### Environments

    ansible-playbook 1-environments.yml
    # will do nothing
    ansible-playbook -i environments/local 1-environments.yml
    # will execute the playbook on localhost
    ansible-playbook -i environments/local-with-group_vars 1-environments.yml
    # overwrites the apache_httpd_port to 66066
