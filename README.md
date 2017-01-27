# Files integrity check

Check integrity of files through md5sum. 
Compare the md5sum of the files on remote system with that present in local system,
to check if there are any changes made in the files over time.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.
```
* Download the project and unzip it
			or
* Clone the project to the local machine.
```

### Prerequisites

```
Install Ansible
	Ubuntu - > sudo apt-get install ansible
	Fedora - > sudo dnf install ansible
```

```
Host file should be present in - /etc/ansible/hosts
```

Example of a hosts file

```

[webserver]
192.168.1.1
[local]
127.0.0.1

```

### How to run ansible-playbook

```
ansible-playbook file_integrity_check.yml
```

### Extra points

In hosts file - 
* webserver - Remote server from which files are downloaded
* local - Local system upon which files are to be checked with.


## Authors

* **Anusha Rao** - [anrao91](https://github.com/anrao91)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* http://docs.ansible.com/ansible/quickstart.html
* http://docs.ansible.com/ansible/playbooks.html
* http://docs.ansible.com/ansible/command_module.html

