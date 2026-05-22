# Port Security Lab

## Objective
Configure Port Security on switch interfaces to control access and restrict unauthorized devices from connecting to the network.

## Topics Covered
- Port Security configuration
- Sticky MAC addresses
- Violation modes
- Secure access control
- Interface protection

## Technologies Used
- Cisco Packet Tracer
- Cisco IOS
- Layer 2 Switching

## Configuration

### Switch Configuration
```bash
enable
configure terminal

interface INTERFACE_ID
switchport mode access
switchport port-security
switchport port-security maximum MAXIMUM_MAC_ADDRESSES
switchport port-security mac-address sticky
switchport port-security violation shutdown

end
```

## Verification Commands
```bash
show port-security
show port-security interface INTERFACE_ID
show running-config
```

## Skills Practiced
- Switch security
- Access control
- MAC address security
- Cisco IOS configuration
- Basic troubleshooting