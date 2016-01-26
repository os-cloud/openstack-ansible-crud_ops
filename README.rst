crud_ops role
#############
:tags: openstack, cloud, ansible, crud_ops
:category: \*nix

Role setup and creation of database and messaging backends that
OpenStack Services depend on.

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
