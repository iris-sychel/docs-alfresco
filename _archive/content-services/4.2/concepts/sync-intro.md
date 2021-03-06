---
author: [Alfresco Documentation, Alfresco Documentation]
audience: 
---

# Configuring synchronization

The synchronization subsystem manages the synchronization of Alfresco with all the user registries \(LDAP servers\) in the authentication chain.

The synchronization subsystem supports three modes of synchronization:

-   **Full**

    All users and groups are queried, regardless of when they were last modified. All local copies of these users and groups already existing are then updated and new copies are made of new users and groups. Since processing all users and groups in this manner may be fairly time consuming, this mode of synchronization is usually only triggered on the very first sync when the subsystem first starts up. However, synchronization can also be triggered in this mode by the scheduled synchronization job, if `synchronization.synchronizeChangesOnly` is set to false.

-   **Differential**

    Only those users and groups changed since the last query are queried and created/updated locally. This differential mode is much faster than full synchronization. By default, it is triggered when the subsystem starts up after the first time and also when a user is successfully authenticated who does not yet have a local person object in Alfresco. This means that new users, and their group information, are pulled over from LDAP servers as and when required with minimal overhead.

-   **Differential With Removals**

    All users and groups are queried to determine which ones no longer exist and can be disabled or deleted locally. In order to synchronize the attributes of the remaining users and groups, a differential sync is performed so only those users and groups that have changed since the last sync are updated or added locally.


-   **[Synchronization triggers](../concepts/sync-triggers.md)**  
Synchronization can be triggered by each of the following events:
-   **[Synchronization deletion](../concepts/sync-delete.md)**  
Users and groups removed from the LDAP directory or query are only identified when synchronization is triggered by the schedule job in either full mode or differential with removals mode.
-   **[../concepts/sync-collision.md](../concepts/sync-collision.md)**  

-   **[Synchronization configuration properties](../concepts/sync-props.md)**  
The synchronization subsystem manages synchronization of Alfresco by configuring the subsystem's properties.

**Parent topic:**[Configuring Alfresco](../concepts/ch-configuration.md)

