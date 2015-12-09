How to install
--------------

    ansible-galaxy install -r requirements.yml

with the content of requirements.yml
    
    
    # requirements.yml
    
    - src: https://github.com/vantt/ansible_java_openjdk.git
      version: master
      name: java_openjdk_role

How to use
----------

    # playbook.yml
    
    - hosts:  all 
      sudo: yes
      gather_facts: true
      roles:
        - { role: java_openjdk_role }
