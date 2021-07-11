zfs-my-commands
**TLDR;** `docker` creates so many zfs datasets and snapshots that makes the vanilla `zfs` command difficult to operate. this fixes that, somewhat.

### description

some helper script for zfs fiesystem
- `zfs-list` lists zfs datasets excluding anything that has the word `docker` in it
- `zfs-list-snapshot` lists zfs snapshots excluding anything that has the word `docker` in it. 

### installation

- become root
- go to `/usr/local/bin`
  ```
  cd /usr/local/bin
  ```
- clone this repo:
  ```
  git clone https://github.com/kongkrit/zfs-my-commands
  ```
- make the commands executable
  ```
  chmod +x zfs-my-commands/scripts/*
  ```
- link them to `/usr/local/bin`
  ```
  ln -fs /usr/local/bin/zfs-my-commands/scripts/* /usr/local/bin
  ```

### uninstallation
- remove all stuff installed above from `/usr/local/bin`
