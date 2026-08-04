# Personal-Packet-Tracer-Labs
This repository features a collection of hands-on Cisco Packet Tracer projects that reflect my growth, skills, and practical experience as I progress on my journey to becoming a network engineer.

I utilized ChatGPT to prompt me for 10 Cisco Packet Tracer Labs from Beginner to Advanced.

# Beginner Labs

Lab 1: Basic Network Setup (2 PCs + Switch) 💻

   - Connect 2 PCs to a Switch
   - Assign IP Addresses manually
   - Test them with ping

       - Ping is a computer network tool used to test connectivity and the distance between two devices. Ping measures the round-trip time it takes for a client to get a response from a server, most often measured in milliseconds. The lower the ping, the faster the response time.


 # Part 1 - Build the topology 🌐
- Add a Switch:
   - Select 'Network Devices' --> 'Switches' --> '2960 IOS15' (model of the Cisco Catalyst 2960 Series Switches). Drag the selection into the center of the workspace.
      
      - 2960-24TT Specifications:
         - Uplink Interfaces: 2 x 10/100/1000 TX uplinks
         - Ports: 24 x Ethernet 10/100 ports
         - Throughput: 6.5 Mbps
         - Backplane Capacity: 16 Gbps
         - DRAM: 16 MB
- Add two PCs:
   - Select 'PC'. Drag two PCs into the workspace.

         - PC0 --- SWITCH --- PC1

# Part 2 - Connect the devices 🔌
- Select cable type:
  - Click the "connections" icon (lightening bolt)
       - Copper Straight-Through
- Connect PC0:
  - click PC0 --> FastEthernet0 then click the switch --> FastEthernet0/1
- Connect PC1:
  - click PC1 --> FastEthernet0 then click the switch --> FastEthernet0/2
- The port lights will usually be orange for a few seconds while the switch initializes. After about 30 seconds, they should turn green.
- Green = Link is up 🟢

# Part 3 - Configure the IP Addresses 🔧
- Click into PC0
  - Desktop --> IP Configuration
  - Select "Static"
       - IP Address: 192.168.1.10
       - Subnet Mask: 255.255.255.0
- Click into PC1
  - Desktop --> IP Configuration
  - Select "Static"
       - IP Address: 192.168.1.11
       - Subnet Mask: 255.255.255.0
