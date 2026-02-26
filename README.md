# SOC-stand-article
My description of setting up a SOC virtual network of 4 machines.

## Mashins
i use 4 virtual maschins:
1. Ubuntu (Rourer):
   1. Sensor (Suricata);
   2. Wazux agent.
2. Ubuntu server:
   1. Wazux server.
3. Windows 11:
   1. Wibe-site (python script).  
4. Kali.

## VirtualBox networcks and IP
1. Ubuntu (Router):
   - SOC-Red - 10.10.10.1/24;
   - SOC-Blue - 10.20.20.1/24;
   - NAT - DHCP.
2. Ubuntu Server:
   - SOC-Blue - 10.20.20.10/24
       - gateway - 10.20.20.1
   - MGMT - 192.168.56.10/24
3. Windows 11:
   - 10.20.20.100/24
       - gateway - 10.20.20.1
4. Kali:
   - 10.10.10.100/24
       - gateway - 10.10.10.1

