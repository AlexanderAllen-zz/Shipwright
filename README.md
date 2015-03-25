Shipwright
==========

Shipwright is a Ansible role that creates development environments for building Docker containers.


Requirements
------------

Operating system:

* Ubuntu 14.04 (Trusty) or greater.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

**Optional**:

* **Docker Hub login credentials**
    * If you are using [Vault](https://github.com/AlexanderAllen/Vault) to manage your 
    [Docker Hub Registry](https://registry.hub.docker.com/) login credentials, store the following variables in your 
    `vault.yml`, and they will be used by Shipwright to automatically log you in to the Docker Hub Registry:
    * `docker_hub_user`: Docker Hub username.
    * `docker_hub_pass`: Docker Hub password.
    * `docker_hub_email`: Docker Hub email.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

**Optional**:

* [AlexanderAllen.Vault](https://github.com/AlexanderAllen/Vault): Generic Ansible Vault implementation. Use Vault to 
store and encrypt [Docker Hub Registry](https://registry.hub.docker.com/) credentials.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:


```yaml
- hosts: Shipyard
  roles:
     - AlexanderAllen.Shipwright
```

License
-------

BSD 3-clause "New" or "Revised" License

Author Information
------------------

**Richard Alexander Allen**

* Github: [github.com/AlexanderAllen](https://github.com/AlexanderAllen)
* LinkedIn: [linkedin.com/in/drupalista](https://www.linkedin.com/in/drupalista)
* Fingerprint: `0F10 80F8 2CC9 4714 92C4  5091 53B6 0008 9A94 FA73`
