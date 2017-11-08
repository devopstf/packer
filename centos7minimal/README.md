# Packer Example - CentOS 7 minimal Vagrant Box using Ansible provisioner

**Current CentOS Version Used**: 7.3

This example build configuration installs and configures CentOS 7 x86_64 minimal using Ansible, and then generates the Vagrant box file for VirtualBox. The example can be modified to use more Ansible roles, plays, and included playbooks to fully configure (or partially) configure a box file suitable for deployment for development environments.

## Requirements

The following software must be installed/present on your local machine before you can use Packer to build the Vagrant box file:

  - [Packer](http://www.packer.io/)
  - [Vagrant](http://vagrantup.com/)
  - [VirtualBox](https://www.virtualbox.org/)
  - [Ansible](http://docs.ansible.com/intro_installation.html)

## Usage

Make sure all the required software (listed above) is installed, then cd to the directory containing this README.md file, and run: ``packer build centos7.json``

After a few minutes, Packer should tell you the box was generated successfully.

If you want to only build a box: ``packer build centos7.json``

## Testing built boxes

There's an included Vagrantfile that allows quick testing of the built Vagrant boxes: ``vagrant up``

## License

MIT license.

## Author Information

Created in 2014 by [Jeff Geerling](http://jeffgeerling.com/), author of [Ansible for DevOps](http://ansiblefordevops.com/).
