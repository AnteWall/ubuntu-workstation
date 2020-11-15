### Install ansible and utils

```bash
sudo apt -y update
sudo apt-get -y install ssh ansible git aptitude wget unzip
```

### Download git repo

```bash
git clone https://github.com/AnteWall/ubuntu-workstation.git
```

### Run script

```bash
ansible-playbook -i "localhost," -c local filename.yml --ask-become-pass 
```

#### `common.yml`

Installs `docker`, `net-tools`, `curl`, `ubuntu-drivers-common`, `nvidia-drivers`

#### REBOOT AFTER THIS SCRIPT

#### `microk8s.yml`

Installs `microk8s`, `kubectl`, `helm`

#### REBOOT AFTER THIS SCRIPT
