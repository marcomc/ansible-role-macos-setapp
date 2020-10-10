[![Build Status](https://travis-ci.com/marcomc/ansible-role-macos-setapp.svg?branch=master)](https://travis-ci.com/marcomc/ansible-role-macos-setapp)

# Ansible role to install SetApp application store
Installs [SetApp](https://setapp.com/) application store via homebrew, removes it from quarantine and launch it.

Once it's launched the user can install all its 'favourite' apps from SetApp.

Used in [Splinter, an opinionated provisioning tool for macOS](https://github.com/marcomc/splinter).

## (Soft) Requirements & Dependencies
* [Jeff Geerling](https://github.com/geerlingguy)'s' [geerlingguy.homebrew](https://github.com/geerlingguy/ansible-role-homebrew) which is defined as Ansible Galaxy dependency

### Ansible
It was tested on the following versions:
 * 2.9

### Operating systems
Target MacOS 10.15 possibly earlier versions too (not yet tested)

## Example Playbook
Just include this role in your list.
For example

    - host: all
      roles:
        - marcomc.macos_setapp

## Variables

### Target User: `target_user_id`
Used in case you want to link the `Setapp` dir to another user `Dock`.

    target_user_id: "{{ ansible_user_id }}" # Options

By defaults it add it to the current user's Dock.

## Continuous integration
This role has (not yet) a travis basic test (for github) only.

## Troubleshooting & Known issues

License
-------
[MIT](LICENSE)

Author : Marco Massari Calderone (c) 2020 - marco@marcomc.com
