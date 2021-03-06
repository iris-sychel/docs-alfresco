---
author: [Alfresco Documentation, Alfresco Documentation]
source: 
audience: 
category: Administration
option: file servers subsystem NFS
---

# Configuring the NFS file server

It is recommended that TCP connections are used to connect to the Alfresco Network File System server. Using a read/write size of 32K will also help to optimize the performance.

NFS is a distributed file system protocol that allows a user on a client to access files over a network. It is an open standard protocol that anyone can implement.

-   **[NFS file server properties](../concepts/fileserv-nfs-props.md)**  
The following properties can be configured for the NFS server.
-   **[NFS advanced Spring overrides](../tasks/fileserv-nfs-adv.md)**  
The NFS server beans are declared in the file-servers-context.xml file in <configRoot\>\\classes\\alfresco\\subsystems\\fileServers\\default.

**Parent topic:**[Configuring file servers](../concepts/fileserv-subsystem-intro.md)

