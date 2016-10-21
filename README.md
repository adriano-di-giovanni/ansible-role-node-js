# Ansible Role: Node.js

[![Build Status](https://travis-ci.org/adriano-di-giovanni/ansible-role-node-js.svg?branch=master)](https://travis-ci.org/adriano-di-giovanni/ansible-role-node-js)

Ansible role for Node.js:

* basic, opinionated install
* build tools install

## Requirements

None.

## Role variables

<table>
  <thead>
    <tr>
      <th>variable</th>
      <th>required</th>
      <th>default</th>
      <th>choices</th>
      <th>comment</th>
    </tr>
  </thead>
  <tbody>
    <td>node_js_version</td>
    <td>no</td>
    <td>6.x</td>
    <td>
      <ul>
        <li>6.x</li>
        <li>5.x</li>
        <li>4.x</li>
        <li>0.12</li>
        <li>0.10</li>
      </ul>
    </td>
    <td>Node.js version</td>
  </tbody>
</table>

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  become: true
  roles:
    - role: adriano-di-giovanni.node-js
      node_js_version: 6.x
```

The `example/` folder contains project files to provision an Ubuntu Trusty VM using Vagrant and VirtualBox.

## License

MIT

## Resources

* https://nodejs.org/en/download/package-manager/
* https://github.com/nodesource/distributions

## Author Information

Adriano Di Giovanni
