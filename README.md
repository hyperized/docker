hyperized.docker
=========

_Installs docker._

Requirements
------------

Ansible 2.6 or above is highly recommended.

Role Variables
--------------

    docker_state: present
    docker_key_url: https://download.docker.com/linux/ubuntu/gpg
    docker_key_id: "0EBFCD88"
    docker_package: docker-ce
    docker_repo_filename: docker
    docker_repo: "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
    docker_daemon: '{}'

Dependencies
------------

    hyperized.package

Example Playbook
----------------

    - hosts: all
      become: yes
      roles:
        - role: hyperized.docker

License
-------

MIT

Author Information
------------------

Gerben Geijteman <gerben@hyperized.net>
