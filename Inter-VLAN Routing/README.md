# Inter-VLAN Routing Lab

## Objective
Configure Inter-VLAN Routing to allow communication between multiple VLANs using a router.

## Topics Covered
- VLAN creation
- Trunk configuration
- Router-on-a-Stick
- Inter-VLAN communication
- Subinterface configuration

## Technologies Used
- Cisco Packet Tracer
- Cisco IOS
- VLANs
- Router-on-a-Stick

## Configuration

### Switch Configuration
```bash
enable
configure terminal

vlan VLAN_ID
name VLAN_NAME

interface INTERFACE_ID
switchport mode access
switchport access vlan VLAN_ID

interface TRUNK_INTERFACE
switchport mode trunk

end
```

### Router Configuration
```bash
enable
configure terminal

interface INTERFACE.SUBINTERFACE
encapsulation dot1Q VLAN_ID
ip address IP_ADDRESS SUBNET_MASK

interface PHYSICAL_INTERFACE
no shutdown

end
```

## Verification Commands
```bash
show vlan brief
show interfaces trunk
show ip interface brief
ping
```

## Skills Practiced
- VLAN segmentation
- Trunking
- Inter-VLAN Routing
- Router subinterfaces
- Network troubleshooting