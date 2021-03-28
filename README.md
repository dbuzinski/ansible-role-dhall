Dhall
=========

An Ansible Role that installs Dhall Configuration Language. This Role also includes the dhall-to-json, dhall-to-yaml, and json-to-dhall tools.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    nodejs_version: "1.38.1"

The version of Dhall to install. "1.38.1" is the default and works on most supported OSes. 

    dhall_to_json_version: "1.7.6"

This specifies the version of dhall-to-json to install. "1.7.8" is the default and works on most supported OSes. NOTE: This version must be a version included in the Dhall release for dhall_version. See releases here: https://github.com/dhall-lang/dhall-haskell/releases

    windows_install_dir: "%USERPROFILE%\\.dhall"

The directory where the executables will be stored for Windows installations.
Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: dbuzinski.dhall }

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2021 by David Buzinski.