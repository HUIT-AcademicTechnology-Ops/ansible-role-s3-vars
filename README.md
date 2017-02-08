Ansible Role: s3 vars
=========

Retrieve config as a YAML or JSON file from an s3 bucket as an alternative and converts that to playbook vars, as an alternative to using the ansible vault.

Requirements
------------

* boto
* caller needs read access on bucket and config file being requested

Role Variables
--------------

* s3_vars_file_dest: where s3 file is stored locally, defaults to /tmp
* s3_vars_bucket: the s3 bucket where yaml/json file is located
* s3_vars_object: path/to/YAML/OR/JSON/file in bucket

Dependencies
------------

N/A

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------
MIT
