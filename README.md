# tgproxy-ansible
Up telegram proxy with ansible playbooks

### Usage
1) Update ansible roles
`ansible-galaxy install -r requirements.yml`
2) Install base requirements on host if need
`ansible-playbook -i inventory play-docker-base.yml`
3) Up telegram proxy container with predefined secrets
`ansible-playbook -i inventory play-tgproxy.yml --ask-vault-pass`
