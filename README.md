# Ansible Playbook for SoftEther VPN server

see **[SoftEther VPN Project](https://www.softether.org)**


## Requirement

- [Ansible](https://www.ansible.com) (`pip3 install ansible`)


### Server requirement

- OS: Ubuntu 18.04


## Usage

1. Install `community.general.ufw`
    ```sh
    ansible-galaxy collection install community.general
    ```

1. Update `./hosts`
    ```
    vi ./hosts
    ```
    You should change `your-server-host` to your **[Host](http://man7.org/linux/man-pages/man5/ssh_config.5.html)**
    
1. Deploy
    ```sh
    ansible-playbook -i hosts vpn.yml
    ```
