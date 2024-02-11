requires `apt install git ansible -y`

implied: requires passwd set for *username* in bootstrap lines 14, 15, 27

implicit: ansible-playbook 03-docker-directories.yml && sh 04-install-docker.sh && sh 05-install-docker-containers.sh && ansible-playbook 06-install-tools.yml && ansible-playbook 08-create-dirs.yml

