# Hacktalk Wolfsburg - Ansible
## Part 4: a complete sample
This playbook installs Apache HTTPD and sets up a few websites.

## Execute

	# we have two environments: "local" and "vm"
	# to keep our local environment clean, we execute the role on the remote instance
    sudo ansible-playbook -i environments/vm webserver.yml --step
