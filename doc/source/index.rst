crud_ops Docs
=============

This role simply creates and does a basic setup for anything
CRUD related that a given OpenStack service may need.

Basic Role Example
^^^^^^^^^^^^^^^^^^

Tell us how to use the role.

.. code-block:: yaml

    - name: Playbook for role testing
      hosts: localhost
      connection: local
      roles:
        - role: "crud_ops"
          mysql_root_user: root
          mysql_root_password: secrete
          mysql_address: localhost
          mysql_database: testing
          mysql_user: test
          mysql_password: SuperSecreteTesting
          mysql_delegate_to: localhost
          rabbitmq_vhost: /testing
          rabbitmq_userid: testing
          rabbitmq_password: SuperSecreteTesting
          rabbitmq_delegate_to: localhost
