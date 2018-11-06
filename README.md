
# Install:

    pipenv install ansible ansible-runner
    pipenv shell
    ansible-galaxy install benthomasson.vagrant_tools -p roles

# Start:

    ansible-playbook -i localhost -vvvv up.yml

# Ping with vagrant key:

     ansible-runner -m ping --hosts all --inventory ./hosts run private_data_dir

# Ping with generated key:

    <generate ssh key in files key and key.pub>
    ssh-keygen -f key
    ssh-add key
    ansible-playbook -i hosts key.yml
    ansible-runner -m ping --hosts all --inventory ./hosts2 run private_data_dir
