Erlang-Relx
========

This role will install Erlang relx from [relx](https://github.com/erlware/relx.git).

Requirements
------------

This role requires Ansible 1.4 or higher, and platform requirements are listed in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows:

* `erlang_relx_git`: location of the relx git repository [default: `https://github.com/erlware/relx.git`]
* `erlang_relx_src_path`: where to clone the relx git repository [default: `~/src/relx`]
* `erlang_relx_version`: relx version to install [default: `v0.6.0`]
* `erlang_relx_bin_path`: where to store the relx binary [default: `~/bin/relx`]

Example Playbook
-------------------------

    - hosts: all
      roles:
         - { role: rymir.erlang-relx, erlang_relx_version: v0.6.0 }

Dependencies
------------

[Ansibles.erlang](https://galaxy.ansible.com/list#/roles/541)

License
-------

MIT

Author Information
------------------

rymir
