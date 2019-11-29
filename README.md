# Ansible Proxmox KVM agent_info

Test playbook to show working example of `agent_info` feature of Proxmox KVM module.

## Usage

Start VM for which you want fetch data. Make sure it has installed and enabled QEMU Guest Agent. If you see IPs section shown (with actual IPs assigned to VM) inside PVE web GUI, then it means everything works as expected. Now clone this repo and cd into dir, then run ...

```
$ ansible-playbook playbook.yml
```

... and correctly fill out all prompt vars. Upon successful execution you'll see the result of data which was fetched via QEMU Guest Agent feature.
