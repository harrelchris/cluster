# Cluster

## Contents

- Requirements
- Installation
- Web UI
- Cluster
- Shared Storage
- High Availability
- ISOs
- Templates

## Requirements

- [Proxmox VE](https://www.proxmox.com/en/downloads)
- [Rufus](https://rufus.ie/en/)
- USB Drive

## Dell Optiplex

- Bios: F2
- Boot Menu: F12

## Installation

- Enter boot menu
- Select USB
- Select Install Proxmox GUI
- Enter the following:

  Field | Value
  ---|---
  Terms | Agree
  Drive | Select (Default)
  Country | United States
  Timezone | America/Chicago
  Password | 
  Email | harrelchris@gmail.com
  Hostname | ⚠️ pve1.example
  IP Address | ⚠️ 192.168.18.101 
  Gateway | 192.168.18.1
  DNS Server | 1.1.1.1

  ⚠️ Different for each node

- Reboot
- user: `root`
- `shutdown now`

## Web UI

[https://192.168.18.101:8006](https://192.168.18.101:8006)

## Cluster

## Shared Storage

### Synology NFS

https://www.youtube.com/watch?v=EMQdN6W_y1Y

1. Enable NFS
  1. Control Panel
  1. File Services
  1. NFS
  1. Enabled
1. Create volume
  1. Control Panel
  1. Shared Folder
  1. Create
  1. Disable Recycle Bin
1. Create an NFS rule
1. Edit Proxmox folder > NFS Permissions > Create
  1. Hostname of Proxmox node

## High Availability

## ISOs

- [Alpine](https://alpinelinux.org/downloads/)
- [Debian](https://www.debian.org/distrib/)
- [Fedora](https://fedoraproject.org/server/download)
- [Ubuntu](https://ubuntu.com/server)

## Templates
