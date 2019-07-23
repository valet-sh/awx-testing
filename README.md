[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)




## Introduction

This project aims to provide automatic installation tests for our [native Debian AWX packages](https://github.com/valet-sh/awx-build-deb) 


## Requirements

ansible and lxd have to be installed on your system

### Testing installation

simply run one of the available playbooks. A new LXD container is created, awx and all required services are installed. The container will be automatically deleted if the install process was successful. More automated tests are planned (e.g. login test, starting a job).

```
ansible-playbook playbooks/awx-debian10-experimental.yml
ansible-playbook playbooks/awx-debian10-testing.yml
ansible-playbook playbooks/awx-debian10-stable.yml
```


## License


[Apache v2](./LICENSE.md)
