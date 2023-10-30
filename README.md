### Initialize

1. comment the following line from the cross_env.yml `ansible_python_interpreter: "{{ venv_path }}/bin/python"`
2. run the playbook with `initial` tag `ansible-playbook -i provisioning/environments/prod/ provisioning/playbook.yml -t initial`
3. after the playbook successful run uncomment the line from step 1 and run the playbook again without the initial tag  `ansible-playbook -i provisioning/environments/prod/ provisioning/playbook.yml`