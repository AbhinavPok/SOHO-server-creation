# Home Server: NAS + Security System

This project demonstrates how I converted an old laptop into a fully functional server that acts as:
- **NAS (Network Attached Storage)** for centralized file storage and backup
- **Home Security System** with camera integration and monitoring

The goal is to repurpose old hardware into a **low-cost, efficient, and secure server**, while documenting setup steps, configurations, and security best practices.

```
Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#hostname SW1
SW1(config)#ip default-gateway 192.168.1.254
SW1(config)#interface vlan 1
SW1(config-if)#ip address 192.168.1.200 255.255.255.0
SW1(config-if)#no shutdown
SW1(config-if)#end
SW1#
*Mar  1 00:03:44.261: %SYS-5-CONFIG_I: Configured from console by console
SW1#copy running-config startup-config
Destination filename [startup-config]?
Building configuration...
[OK]
0 bytes copied in 1.141 secs (0 bytes/sec)
SW1#
```
  
    
