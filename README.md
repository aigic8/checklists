# Checklists

My personal lists of checklists for repetitive tasks to not to forget one.

## List

- [Setting up a server](#setting-up-a-server)

## Setting up a server

- upgrade server
  - [Fedora](https://docs.fedoraproject.org/en-US/quick-docs/upgrading-fedora-offline/)
- create a non-root user

```bash
useradd -m USERNAME
```

- add password to non-root user

```bash
passwd USERNAME
```

- [install zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)
- configure ssh
  - add local ssh key to server root (change the key file if it is not `id_ed25519.pub` for you)
  ```bash
  ssh-copy-id -i ~/.ssh/id_ed25519.pub root@server_address
  ```
  - add local ssh key to server (change the key file if it is not `id_ed25519.pub` for you)
  ```bash
  ssh-copy-id -i ~/.ssh/id_ed25519.pub username@server_address
  ```
  - [disable password based authentication](https://linuxhandbook.com/ssh-disable-password-authentication/)
- [change the default ssh port](https://linuxize.com/post/how-to-change-ssh-port-in-linux/)
- [add ssh config to your local machine](https://linuxize.com/post/using-the-ssh-config-file/) (OPTIONAL)
- [install OhMyZSH](https://ohmyz.sh/#install)
- install basic packages
  - git
  - neovim
  - tmux
  - curl
  - unzip
  - [Node.js (fnm)](https://github.com/Schniz/fnm)
  - [bun](https://bun.sh/docs/installation#macos-and-linux)
  - [Go](https://go.dev/doc/install)
  - docker
    - [Fedora](https://developer.fedoraproject.org/tools/docker/docker-installation.html)
    - add non-root user ability to run docker `usermod -aG docker USERNAME`
- setup firewall (TODO) (OPTIONAL)
  - don't forget to **add the custom SSH port to firewall**
- setup neovim configs from [dotenv](https://github.com/aigic8/dotenv)
- setup tmux from [dotenv](https://github.com/aigic8/dotenv)
