
# Install:

    pipenv install ansible ansible-runner
    pipenv shell
    ansible-galaxy install benthomasson.vagrant_tools -p roles

# Start:

    ansible-playbook -i localhost -vvvv up.yml
