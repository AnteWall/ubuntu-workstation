### Install ansible and utils

```bash
sudo apt -y update
sudo apt-get -y install ssh ansible git aptitude wget unzip
```

## Run script

```bash
ansible-playbook -i "localhost," -c local filename.yml --ask-become-pass 
```