Jenkins Ansible Idempotency Testing
===================================

An introduction on using vagrant, Jenkins, and docker to test the idempotency of [Ansible] playbooks.

[ansible]: http://www.ansible.com/

## Requirements

You must have ansible installed on your system.

[Installation instructions]

[Installation instructions]: http://docs.ansible.com/intro_installation.html

You must then install the [Jenkins ansible-galaxy] role:

[Jenkins ansible-galaxy]: https://galaxy.ansible.com/list#/roles/440

```
ansible-galaxy install geerlingguy.jenkins
```

## Quick Start

1. Clone this repository ```git clone https://github.com/tylerturk/jenkins_ansible_idempotent_test.git```
2. cd in to the repository directory ```cd jenkins_ansible_idempotent_test```
3. Bring your vagrant online ```vagrant up```
4. Navigate to [your local jenkins] on your computer
5. Profit?!?!?!
6. Tweet about how awesome testing ansible is.
7. Thank [@geerlingguy] for writing the [Jenkins ansible-galaxy] role

[@geerlingguy]: https://twitter.com/geerlingguy
[your local jenkins]: http://localhost:8080
