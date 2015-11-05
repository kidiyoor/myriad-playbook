# myriad-playbook

Ansible Playbook for setting up Myriad development environment
- Mesos
- Hadoop
- Myriad

Require ansible version >= 1.9

ansible-playbook -i hosts site.yml --private-key=<path>

build.yml : Run each time source code is changed. (Build the myriad jar and copy the JAR to appropriate locations)
restart-master.yml : Restart Resource manager.

status: in progress

TODO 
- copy JAR to slaves
- configure yarn-site.xml (myriad/tasks/main.yml)
- use snsible vault for password
