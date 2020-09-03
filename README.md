# Ansible role to install SetApp application store
Installs [SetApp](https://setapp.com/) application store via homebrew, removes it from quarantine and launch it.

Once it's launched the user can install all its favourite apps from SetApp.

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
        - marcomc.setapp

## Variables

No variable required.

## Continuous integration
This role has (not yet) a travis basic test (for github) only.

## Troubleshooting & Known issues

## Copyright
Marco Massari Calderone (c) 2020

## License
MIT
