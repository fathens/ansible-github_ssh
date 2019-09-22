# ansible-github_ssh
Ansible role for registering ssh_key to github

## environment variables

| name | required? | description |
|---|---|---|
| GITHUB_ACCESS_TOKEN | no | Personal access token in Developer settings |

if `GITHUB_ACCESS_TOKEN` is not defined, all tasks will be skipped.
Note that access token requires "Full control of user public keys".

## vars

| name | required? | description |
|---|---|---|
| github_ssh_key_name | no | key file name in ~/.ssh (default: github) |
| github_account.name | no | user's name in ~/.gitconfig |
| github_account.email | no | email in ~/.gitconfig |

Put ~/.gitconfig only if github_account is defined.
