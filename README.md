mfitbs-ansible-ssh
=========

Copies pointed ssh public keys to a remote host also restricts access to sshd. 

Requirements
------------

* Ansible 2.8.5
* Debian 9

Role Variables
--------------

* ssh_keys_dir - local keys dir 
* pub_keys - pub keys list in ssh_keys_dir to copy


Dependencies
------------

N/A

Example Playbook
----------------


    - name: Test
      hosts: server
      roles:
        - role: farynam.mfitbs_ansible_ssh
          vars:
            ssh_keys_dir: conf/mfitbs-ansible-ssh/ssh-keys
            pub_keys:
              - marcin.pub
              ....
      tasks:

License
-------

MIT

Author Information
------------------

Marcin Faryna
