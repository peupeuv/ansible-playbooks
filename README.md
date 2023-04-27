# ansible-playbooks
Collection of Ansible playbooks and roles for automating server configuration and management. Includes playbooks for common tasks such as dotfile deployment, webserver setup, and package management, as well as roles for configuring specific services and applications.
## Steps
To deploy the dotfiles and configure the tools using Ansible, follow these steps:
1. Install Ansible on your local machine:
```
    sudo apt-get update
    sudo apt-get install ansible
```
Replace `apt-get` with the appropriate package manager for your operating system.

Or

use pip in your selected Python environment to install the Ansible package of your choice for the current user:
```
    python3 -m pip install --user ansible
```
2. Clone the repository to your local machine:
```
    git clone https://github.com/yourusername/dotfiles.git
```
3. Update the `inventory.yml` file with the IP addresses and usernames of your remote servers.
4. Run the Ansible playbook to deploy the dotfiles and configure the tools:
```
    cd dotfiles/ansible
    ansible-playbook -i inventory.ini starship-deploy.yml
```
This will install and configure Starship on all remote servers, and deploy your custom configurations from the `dotfiles` repository.
5. Restart your shell or reload the configuration files for the changes to take effect.
## Customization
Feel free to customize the configuration files to match your personal preferences and requirements. If you make any changes, remember to commit and push them back to your repository to keep it up to date.
## Contributing
If you have any suggestions or improvements, feel free to fork the repository, make your changes, and submit a pull request. I'm always open to new ideas and contributions.
## License
This repository is licensed under the [MIT License](LICENSE).
