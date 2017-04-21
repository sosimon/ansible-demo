# Fun with Ansible and EC2

## Prereqs

Prepare virtuaenv environment and install required Python packages
```
virtualenv env
pip install -r requirements.txt
```

Set AWS access and secret keys
```
set AWS_ACCESS_KEY=<key>
set AWS_SECRET_KEY=<key>
```

## Usage

`ansible-playbook -i inventory start.yml`

Note: `-i inventory` is a workaround so ansible will use the right Python in a virtualenv - https://www.zigg.com/2014/using-virtualenv-python-local-ansible.html
