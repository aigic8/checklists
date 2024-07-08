# Setting up a server

## Checklist

- create a non-root user
- setup password-less login for the root
- setup password-less login for the user
- install basic packages
  - neovim
  - curl
  - node.js
  - bun
  - golang
  - docker
    - add non-root user ability to run docker `usermod -aG docker USERNAME`
- setup neovim configs
- setup firewall
