# jsyang's Ansible stuff for OctoPrint on RP0W

### Setting up the host correctly

Add in your info for the `hosts` file before you do this.

```
brew install http://git.io/sshpass.rb
brew install ansible
sudo mkdir -p /etc/ansible
sudo cp hosts /etc/ansible
```

### Running

```
# Add -vvv to the end of any command to increase verbosity

# Start up
ANSIBLE_PIPELINING=True ansible-playbook startup.yml

# Shut down
ANSIBLE_PIPELINING=True ansible-playbook shutdown.yml

# Restart
ANSIBLE_PIPELINING=True ansible-playbook restart.yml

```
