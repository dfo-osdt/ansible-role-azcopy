# Ansible Role Azcopy

## Role Description

`ansible-role-azcopy`: A simple role to install Microsoft's Azure Copy (azcopy)
on Ubuntu.  The role uses the Linux Software Repository for Microsoft Product to
install is as per the instructions found in the azcopy
[documentation](https://learn.microsoft.com/en-us/azure/storage/common/storage-use-azcopy-v10?tabs=dnf#install-azcopy-on-linux-by-using-a-package-manager).


## Requirements

This role is for Ubuntu only.

## Role Variables

- `azcopy_version`: Version of AzCopy to install (default: `latest`)
  - Set to `latest` to install the newest available version (may include preview versions)
  - Set to a specific version to pin, e.g., `10.29.1` for stable releases
  - Use `apt-cache madison azcopy` to see available versions

## Dependencies

No dependencies
