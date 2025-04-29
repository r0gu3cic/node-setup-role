# NODE-SETUP-ROLE

=========

This Ansible role is designed for setting up Node.js, npm, and n on an Ubuntu server. This role prepares the server for production use, enabling efficient management and deployment of Node.js-based applications.

## Requirements

------------

This role is designed to work with Ubuntu distributions. It requires the following:

- Ansible 2.10.8 or higher
- `sshpass` for running the playbook with SSH password authentication.

## Role Variables

------------

The following variables can be configured for this role:

- **`node.version`**: The major version of Node.js we want installed.
- **`node.specific`**: The minor version of Node.js we want installed.

These variables can be defined in the playbook or in a `vars` file.

## Dependencies

------------

This role has no dependencies on other roles.

## License

------------

MIT Licence

## Testing Guide

------------

To run a local test for this role, use the following command:

```bash
ansible-playbook tests/test.yml -i tests/local_inventory.ini -u root -k --extra-vars "hosts=local_vm"
```

## Author Information

------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
