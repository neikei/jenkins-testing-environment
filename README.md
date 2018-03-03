# jenkins-testing-environment

Jenkins testing environment in a Vagrantbox based on Debian and provisioned with Ansible.

## Requirements

- Virtualbox >= 5.2.4
- Vagrant >= 2.0.1
- Vagrant Plugins:
  - vagrant plugin install vagrant-hostmanager
  - vagrant plugin install vagrant-vbguest

## Getting started

1. git clone https://github.com/neikei/jenkins-testing-environment.git
2. cd jenkins-testing-environment
3. vagrant up
4. ... wait ...
5. Open Jenkins in your web browser: http://jenkins.test

## Initial admin password

The initialAdminPassword  is required for the first access to the Jenkins GUI and shown during the provisoning.

```bash
TASK [jenkins : Check initialAdminPassword] ************************************
changed: [default]

TASK [jenkins : Show initialAdminPassword] *************************************
ok: [default] => {
    "msg": "4e57e3a448fc4dd888afeaeffa708368"
}

RUNNING HANDLER [nginx : restart nginx] ****************************************
changed: [default]

PLAY RECAP *********************************************************************
default                    : ok=27   changed=18   unreachable=0    failed=0
```

## Feedback, Issues and Pull-Requests

Feel free to report issues, fork this project and submit pull requests.