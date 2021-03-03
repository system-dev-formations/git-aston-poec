#  GIT TRAINING COURSE
## Pre-requisite for UBUNTU 20.04



##  Install Docker with  Ansible 
### Install Python 
```
sudo apt install -y python3-venv
```

### Set up a python virtualenv, and install ansible
```shell script
  # in the jenkins-pic directory 
  git clone   https://github.com/<your_github_account>/git-aston-poec.git
  cd git-aston-poec
  python3 -m venv venv  # install virtualenv module dans la directory venv
  python -V # check python version
  source venv/bin/activate # activate the python virtualenv
  pip3 install wheel  # install pip package wheel for permission usage
  pip3 install --upgrade pip
  pip3 install ansible # install ansible
  ansible --version  # check, should be version 2.10.6
```

### Run the playbook
```
  ansible-playbook -i inventory  install_docker_ubuntu.yml
```

Please log out and log in again of your shell screen for 
the changes take effect. 
```shell script
   docker ps    # check if docker is up and running 
```

