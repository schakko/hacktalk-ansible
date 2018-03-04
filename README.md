# Hacktalk Wolfsburg - Ansible
## Part 2: Roles and tags

### Roles

    ansible-playbook 1-roles.yml --step

### Tags

    ansible-playbook 2-tags.yml
    # executes both roles
    ansible-playbook 2-tags.yml --tags tagged_role
    # executes only second role

### Tags inheritance

    ansible-playbook 3-tags-inheritance.yml
    # execute all roles
    ansible-playbook 3-tags-inheritance.yml --tags tagged_role
    # execute only second and third role

### Roles with default variables

    ansible-playbook 4-role-with-defaults.yml
    # sets the port to 80
    ansible-playbook 4-role-with-defaults.yml -e apache_http_port=10100
    # sets the port to 10100 

