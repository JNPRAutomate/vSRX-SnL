vSRX Square
=================

A topology containing two vSRXs that can be used to interoperate with each other

Topology
========

The topology consists of seven VMs: seven vSRXs. Thes vSRX are configured in a spine and leaf topology. Where each leaf node is connected to each spine node.

```

Insert diagram here

```

## Interface Numbering

10.(1-5, LeafID).(1-2, SpineID).(1 Spine, 2 Leaf)

### Access Note

For NETCONF testing each node has its NETCONF port exposed via port forwarding.

- vSRX1 - 8831
- vSRX2 - 8832
- vSRXA - 8833
- vSRXB - 8834
- vSRXC - 8835
- vSRXD - 8836
- vSRXE - 8837

### Vagrant Note

Do to the inner workings of Vagrant each host has a virtual NIC connected back to the host running the virtual machines. This allows Vagrant to provision and control each VM over the SSH protocol. These interfaces are depicted on the topology above.

To use this lab with VMware Fusion or Workstation you must first purchase and install the Vagrant VMware Plugin.

[Vagrant VMware Plugin](https://www.vagrantup.com/vmware)

**VM Access Information**

-	[VM Host Passwords](https://github.com/JNPRAutomate/vSRX-Square/blob/master/docs/vmpasswords.md)
