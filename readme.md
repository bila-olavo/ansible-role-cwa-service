AWS Cloud Watch Agent - CWA
=========

This role will install AWS Cloud Watch Agent reponsible for pushing Custom Metrics to Cloud Watch on Debian (64-bit)

Requirements
----------------

- Operation System: Debian

Example Playbook
----------------


    name: Execute aws-cloudwatch-service Role
    hosts: role.aws-cloudwatch-service
    strategy: free
    gather_facts: yes
    become: yes
    roles:
    - { role: collins.aws-cloudwatch-service, tags: [ 'cloudwatch-agent-service'] }}

Author Information
------------------

https://github.com/bila-olavo/ansible-role-cwa-service
