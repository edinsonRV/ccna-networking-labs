\# VLAN Configuration Lab



\## Objective

Configure VLANs and trunk encapsulation to enable communication between switches across multiple VLANs.



\## Topics Covered

\- VLAN creation

\- Access port configuration

\- Trunk configuration

\- Trunk encapsulation

\- VLAN management



\## Technologies Used

\- Cisco Packet Tracer

\- VLANs

\- Trunking

\- Layer 2 Switching



\## Configuration



\### Switch Configuration

```bash

enable

configure terminal



vlan VLAN\_ID

name VLAN\_NAME



interface INTERFACE\_ID

switchport mode access

switchport access vlan VLAN\_ID



interface TRUNK\_INTERFACE

switchport trunk encapsulation dot1q

switchport mode trunk



end

```



\## Verification Commands

```bash

show vlan brief

show interfaces trunk

show running-config

```



\## Skills Practiced

\- VLAN segmentation

\- Trunk configuration

\- Switch management

\- Layer 2 networking

\- Basic troubleshooting

