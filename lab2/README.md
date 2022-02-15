=== Overview

New monolithic Ansible playbook, `main.yml` and supporting files  which is designed for teaching and training in refacoring and
the use of roles, collections etc.

Designed to replace the function of the old link:https://github.com/tonykay/bad-ansible[`bad-ansible`] with a different
approach, i.e. start with a fully functional playbook and teardown and iteratively refactor.


==== Quick Start

Assumes a configuration matching an AgnosticD `three-tier-app` with a `devops` service account.

=== Outline of main flow

* common
** setup repos (via satellite)
** setup firewalld
* setup postgres
** firewalld rule opening 5432
** install postgres 10
** no data load phase - come back to that?
* setup app tier
** firewalld rule opening 443

=== Development Environment

While intended to be deployed on a _real_ cloud or virtualization platform it
comes with a Vagrantfile and associated playbooks

==== Deploying the Database Tier


=== Notes:

Does firewalld need to be configured?

=== Resources

* Jeff Geerling's Ansible Galaxy Role
* Useful articles on Postgres
** Setting it up from scratch

https://opensource.com/article/17/6/ansible-postgresql-operations
