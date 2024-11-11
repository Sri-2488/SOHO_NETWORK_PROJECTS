# Simple_SOHO_NETWORK
This project demonstrates a basic SOHO (Small Office Home Office) network setup using Cisco Packet Tracer. It showcases essential network engineering skills, such as designing a network, configuring devices, and ensuring connectivity.

## Network Topology

<img width="670" alt="Screenshot 2024-11-11 112304" src="https://github.com/user-attachments/assets/3892a548-d55f-45f8-9e27-ba38ab593789">

## Hardware and Software Requirements
- Cisco Packet Tracer (Version 8.2.2 or higher)
- Router (ISR4331) - Main router connecting internal and external networks
- Wireless home Router - router connecting wireless devices
- Switch (2960-24TT)- Provides connectivity for internal devices
- Server- Configured for DHCP
- PCs, Laptop, Smartphone- End devices in the network

## Network Configuration
<img width="361" alt="image" src="https://github.com/user-attachments/assets/6ee3e29b-6cc9-40ea-ae6d-78f5a5cbefc4">

## Configuration Guide
The below are the Configuration Screenshots of all the devices in the network.
- Router:
  <img width="551" alt="image" src="https://github.com/user-attachments/assets/8ac5b2c0-9612-41ed-b42c-d9d125307479">
- Switch:
  <img width="559" alt="18-vlan config" src="https://github.com/user-attachments/assets/a083483f-0f7d-4b80-ba01-524b6f49847b">
- Server:
<img width="551" alt="17-server" src="https://github.com/user-attachments/assets/290a18ca-5442-4f00-91d4-30e89b410c6b">
<img width="530" alt="image" src="https://github.com/user-attachments/assets/2604a33c-fe2b-4c50-a9df-c16af1eabeb3">
- PC0:
<img width="529" alt="image" src="https://github.com/user-attachments/assets/012ecd38-2801-4dc3-b6a9-93bc8d9c9fe2">
- PC1:
<img width="530" alt="image" src="https://github.com/user-attachments/assets/6c6ca86d-1c1e-426a-b51d-db80fbe12dba">
- Wireless Router:
<img width="578" alt="2" src="https://github.com/user-attachments/assets/264c9710-be26-49c5-80d4-ff1c82007748">
<img width="613" alt="3" src="https://github.com/user-attachments/assets/48ff3e96-6d20-4513-ac51-15e89e2b621d">
<img width="600" alt="4" src="https://github.com/user-attachments/assets/6869f2b1-c015-43ba-8783-04a7858dc891">
- Laptop:
<img width="554" alt="image" src="https://github.com/user-attachments/assets/31274312-627c-469f-891a-0c73bfe526c0">
- Smartphone:
<img width="537" alt="image" src="https://github.com/user-attachments/assets/77f4b39b-a788-441f-a7d2-b00ae6f31923">

## Testing and Validation:
- Ping Test from PC0:
  <img width="536" alt="image" src="https://github.com/user-attachments/assets/6baf51e4-16df-4cdc-a833-9655f6c11dcd">
- Ping Test from PC1:
  <img width="554" alt="image" src="https://github.com/user-attachments/assets/786604ff-ef3f-4820-a08b-0d36a53e9914">
- Ping Test from Server:
  <img width="529" alt="image" src="https://github.com/user-attachments/assets/aecf0e71-85ae-4a60-8dc8-d9f42846920c">
- Ping test from Switch:
  <img width="580" alt="image" src="https://github.com/user-attachments/assets/6d03089c-c2a3-4e29-8909-12bf43d10cea">
- Ping test from router:
  <img width="536" alt="image" src="https://github.com/user-attachments/assets/4c189ef1-10d5-4b13-b049-5465e0fdcc51">
- Ping test from Laptop:
  <img width="541" alt="image" src="https://github.com/user-attachments/assets/156cd2b3-7cb0-4513-8083-fe2aa3b30f14">
- Ping test from Smartphone:
  <img width="554" alt="image" src="https://github.com/user-attachments/assets/27551ff0-9812-46a9-b0ff-f60fbc13c81d">
  
## Troubleshooting
- Issue: Devices are not receiving IP addresses via DHCP.
  Solution: Check the DHCP pool configuration on the router. Ensure the correct network and default gateway are specified.

- Issue: Unable to ping across subnets.
  Solution: Verify router interface configurations and that they are in the "no shutdown" state.

- Issue: Wireless devices cannot connect to the network.
  Solution: Check wireless router settings, ensure SSID is visible, and DHCP is enabled on the wireless router.

## Future Improvements
- Add VLANs: Separate devices into VLANs for enhanced network segmentation and security.
- Implement Security: Configure ACLs, port security on the switch, and WPA2 security for wireless networks.
- Add NAT: Configure Network Address Translation if you simulate an external network.




