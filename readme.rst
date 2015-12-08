TEMPLATE role
#############
:tags: openstack, cloud, ansible, TEMPLATE
:category: \*nix

TEMPLATE Role

.. code-block:: yaml

    - name: TEMPLATE role
      hosts: "hosts"
      user: root
      roles:
        - { role: "TEMPLATE" }


Note. The template role has the template name within it. Please change the name 
throughout the code base.

.. code-block:: bsah

    find . -type f -exec sed -i 's/TEMPLATE/CHANGE_ME_PLEASE/g' {} \;
