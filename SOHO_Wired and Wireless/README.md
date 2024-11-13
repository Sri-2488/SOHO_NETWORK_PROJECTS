
# SOHO Wired and Wireless Network using DHCP and RADIUS

## Project Overview
This project demonstrates the design and configuration of a Small Office/Home Office (SOHO) network topology, aimed at segmenting employee and guest networks while ensuring secure access management. The setup includes dynamic IP allocation via DHCP, network segmentation using VLANs, and secure wireless authentication through a RADIUS server. This project showcases foundational networking concepts and practical configurations of various network devices.

## Network Topology
<img width="707" alt="image" src="https://github.com/user-attachments/assets/9618371d-d142-421a-8520-25aa7b20128a">

The network consists of two primary VLANs:
- **VLAN 10 - Employee Network**: Designed for internal staff, this VLAN connects both wired and wireless devices within the company network. Devices within this VLAN have access to company resources and receive IP addresses dynamically through a dedicated DHCP server.
- **VLAN 20 - Guest Network**: Created for guests and visitors, this VLAN is isolated from the employee network for enhanced security. Devices in this VLAN receive IP addresses through the DHCP service on the wireless router and have internet access but no access to internal resources.

### Components
1. **DHCP Servers**:
   - **Internal Employee Network**: A dedicated DHCP server is configured to assign IP addresses to devices within the Employee VLAN (VLAN 10) using the `192.168.10.0/24` range.
   - **Guest Network**: The wireless router provides DHCP services for the Guest VLAN (VLAN 20), assigning IP addresses within the `192.168.2.0/24` range.

2. **RADIUS Server**:
   - Configured to handle secure authentication for **guest users only**. 
   - This RADIUS setup ensures that only authorized guest devices can connect to the guest network, adding an extra layer of security for Wi-Fi access.

3. **Access Points and Wireless Router**:
   - **Access Point (Employee Network)**: Provides wireless access for employees in VLAN 10.
   - **Wireless Router (Guest Network)**: Separates guest traffic and manages DHCP allocation for guests in VLAN 20.

4. **Router and Switches**:
   - **Core Router**: Routes traffic between the Employee and Guest VLANs and enforces inter-VLAN routing policies.
   - **Switches**: Used to interconnect devices within the Employee and Guest VLANs, supporting both wired and wireless connectivity.

## IP Addressing and VLAN Configuration
<img width="320" alt="image" src="https://github.com/user-attachments/assets/c202017b-a917-4f56-8b06-13f9e72bfbd6">

- **VLAN 10 - Employee Network**:
  - IP Range: `192.168.10.0/24`
  - Devices are assigned IP addresses from the DHCP server.
- **VLAN 20 - Guest Network**:
  - IP Range: `192.168.2.0/24`
  - Devices are assigned IP addresses from the wireless router’s DHCP.

## Configuration Summary
- **DHCP Configuration**:
  - Employee devices in VLAN 10 receive IP addresses from a dedicated DHCP server.
  - Guest devices in VLAN 20 are assigned IPs by the wireless router’s internal DHCP.

- **RADIUS Authentication**:
  - Configured on the wireless router for guest users only.
  - Ensures that only authenticated guests are granted access to the Wi-Fi network.

## Troubleshooting
- **DHCP Issues**:
  - Ensure the DHCP server for VLAN 10 is correctly configured with the appropriate IP address pool and that devices are connected to the correct VLAN.
  - Verify that the wireless router’s DHCP service is enabled for guest devices on VLAN 20.

- **RADIUS Authentication**:
  - Verify RADIUS server settings and ensure the wireless router is configured to authenticate guests through the RADIUS server.
  - Check that guest devices are using the correct SSID and credentials for Wi-Fi access.

- **Inter-VLAN Routing**:
  - If devices cannot communicate across VLANs as expected, check the router’s inter-VLAN routing configuration and ensure firewall rules allow necessary traffic.

## Future Improvements
- **Enhanced Security**: Implement access control lists (ACLs) to restrict network traffic between VLANs further, limiting access to only necessary resources.
- **Network Monitoring**: Add network monitoring tools to monitor traffic and detect potential security threats.
- **VPN Access for Remote Employees**: Set up a VPN server to allow secure remote access for employees working from home.
- **Bandwidth Management**: Implement Quality of Service (QoS) policies to prioritize network traffic and improve performance for critical applications.

## Conclusion
This SOHO network topology demonstrates key networking concepts like VLAN segmentation, DHCP configuration, and RADIUS authentication. By creating separate employee and guest networks with secure access control, it showcases effective network organization and security. The project emphasizes the importance of network segmentation and access control, providing a solid foundation in network design for real-world applications.

Feel free to connect with me on [LinkedIn](https://www.linkedin.com) and view more projects on [GitHub](https://www.github.com).   
---
