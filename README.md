# Magudulela_Project_CMPG325

 #Network Topologies Design & Simulation
 
Bus Topology

•	All devices are connected to a single central cable called the bus or backbone.
Data sent by any device travels along the bus to all other devices.
It's simple and cost-effective to set up with less cabling required.
However, if the central bus cable fails, the entire network goes down.
Performance can degrade as more devices are added due to data collisions and traffic on the shared bus.

Star Topology

•	All devices connect individually to a central hub or switch.
Data passes through the hub, which manages traffic and directs it to the intended device.
It is easy to install, manage, and troubleshoot since each device has its own cable.
If one device or its cable fails, it does not affect the rest of the network.
However, the hub is a single point of failure; if it fails, the entire network stops working.
It requires more cabling and is therefore more expensive than bus topology.

Ring Topology

Devices are connected in a circular fashion, with each device connected to two others.
Data travels in one direction around the ring, passing through each device until it reaches the destination.
It's relatively inexpensive to install and can manage data flow fairly evenly.
However, if a single device or connection breaks, the entire network can be disrupted.
Dual ring setups can mitigate failures by sending data in opposite directions.

Mesh Topology

•	In mesh topology, every device (node) is interconnected with every other device, either fully or partially.
Full mesh means each node has a direct link to all other nodes, offering high redundancy and fault tolerance since data can take multiple routes if one path fails.
Partial mesh links some nodes to multiple others without full interconnection, balancing cost and reliability.
This topology supports robust and reliable data transmission but can be expensive and complex to implement due to the large number of connections

Extended Star Topology

•	Extended star topology is an expansion of the star topology where multiple star-configured networks are connected through a central hub or switch.
It essentially links several star networks together to cover a larger area or more devices, maintaining the star benefits at a larger scale.
If one of the connecting hubs fails, it may isolate the entire subsection but individual device failures still only affect their direct connection.
This topology allows scalability with relative ease while maintaining manageable cabling and fault isolation

Hybrid Topology

•	Hybrid topology is a combination of two or more different types of topologies (e.g., star, mesh, bus) integrated into one network.
It leverages the strengths and mitigates weaknesses of the component topologies to suit specific network requirements such as performance, fault tolerance, scalability, and cost.
For example, a large network might use a star topology in some segments and mesh in others where high reliability is critical.
Hybrid topology is flexible and can be adapted to complex environments but may increase network design and management complexity

#Individual Network Feature Configuration

SSH (Secure Shell) and Telnet are both network protocols used for remote access and management of devices but differ significantly in security and functionality.

SSH (Secure Shell)

•	SSH is a cryptographic network protocol that provides secure, encrypted communication over an unsecured network.
It operates by authenticating users through public-key cryptography and encrypting all data transmitted, including passwords and commands, protecting against eavesdropping, tampering, and man-in-the-middle attacks.
Besides remote command-line access, SSH also supports secure file transfers (SFTP) and tunneling other network protocols securely.

Importance: SSH is critical for securely managing servers and network devices remotely, especially over public or untrusted networks, ensuring confidentiality and integrity of data.

Telnet

•	Telnet is an older protocol designed primarily for remote command-line access over a network.
It transmits data, including usernames and passwords, in plaintext without encryption, making it highly vulnerable to interception and attacks.
It uses port 23 by default and lacks robust authentication and security features.
Importance: Telnet was historically important for remote management but is now largely obsolete due to its security flaws and has been replaced by SSH in most scenarios.

Why Telnet Should Be Disabled

•	Telnet sends all data as plaintext, exposing sensitive information to attackers who can easily intercept and steal credentials.
It does not verify the identity of the remote server, leaving users vulnerable to impersonation and man-in-the-middle attacks.
Modern security standards and best practices recommend disabling Telnet in favor of SSH to secure remote administration.
Retaining Telnet could lead to unauthorized access and compromise of networked systems.

