# my-zfs-commands
**TLDR;** `docker` creates so many zfs datasets and snapshots that makes the vanilla `zfs` command difficult to operate. this fixes that, somewhat.

### description

some helper script for zfs fiesystem
- `zfs-list` lists zfs datasets excluding anything that has the word `docker` in it
- `zfs-list-snapshot` lists zfs snapshots excluding anything that has the word `docker` in it. 

### installation

- become root
- clone this repo:
  ```
  git clone https://github.com/kongkrit/my-zfs-commands
  ```
- make the commands executable
  ```
  chmod +x my-zfs-commands/scripts/*
  ```
- link them to `/usr/local/bin`
  ```
  ln -fs ${PWD}/my-zfs-commands/scripts/* /usr/local/bin
  ```

### uninstallation
- remove all the symlinks from `/usr/local/bin`
