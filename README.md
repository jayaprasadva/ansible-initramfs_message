## initramfs_message

[![Travis CI](http://img.shields.io/travis/ypid/ansible-initramfs_message.svg?style=flat)](http://travis-ci.org/ypid/ansible-initramfs_message)
[![Ansible Galaxy](http://img.shields.io/badge/galaxy-ypid.initramfs_message-660198.svg?style=flat)](https://galaxy.ansible.com/list#/roles/2807)
[![Platforms](http://img.shields.io/badge/platforms-debian-lightgrey.svg?style=flat)](#)


Define a message which is shown at boot from the init script (initramfs).

The message should appear shortly after the kernel has mounted the initramfs and starts the init script.

This can be useful to show information (like contact information) from an otherwise completly encrytped system.

### Installation

This role requires at least Ansible `v1.3`. To install it, run:

    ansible-galaxy install ypid.initramfs_message

To install via git, run either:

    git clone https://github.com/ypid/ansible-initramfs_message ypid.initramfs_message
    git submodule add https://github.com/ypid/ansible-initramfs_message roles/ypid.initramfs_message




### Role variables

List of default variables available in the inventory:

    ---
    
    initramfs_message_init_file: "/usr/share/initramfs-tools/init"
    
    # Defines a message which is shown at boot shortly after the kernel has mounted initramfs and starts the init script.
    initramfs_message: "\\n {{ initramfs_message_lang_en }} \\n{{ initramfs_message_lang_de }}\\n"

List of internal variables used by the role:

    initramfs_message_expanded


### Authors and license

`initramfs_message` role was written by:

- [Robin Schneider](https://github.com/ypid) | [e-mail](mailto:ypid@riseup.net)

License: [AGPLv3](https://tldrlegal.com/license/gnu-affero-general-public-license-v3-%28agpl-3.0%29)

***

README generated by [Ansigenome](https://github.com/nickjj/ansigenome/).
