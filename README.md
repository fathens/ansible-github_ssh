# ansible-github_ssh
Ansible role for registering ssh_key to github

## environment variables

| name | required? | description |
|---|---|---|
| GITHUB_ACCESS_TOKEN | no | Personal access token in Developer settings |

if `GITHUB_ACCESS_TOKEN` is not defined, all tasks will be skipped.
Note that access token requires "Full control of user public keys".
