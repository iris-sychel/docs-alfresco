---
author: Alfresco Documentation
---

# `cleanSitePermissions`

`cleanSitePermissions()` these methods clean permissions from a node.

When a node is moved or copied from one site to another, the node will retain associated permissions assigned in the source site. These methods allow any permission from outside of the current site to be removed, so that only the permissions of the containing site will apply to the specified node.

**Parent topic:**[Site service object](../references/API-JS-SiteserviceObject.md)

## `cleanSitePermissions(ScriptNode targetNode)`

`cleanSitePermissions(ScriptNode targetNode)` cleans permissions from the node specified by the supplied ScriptNode object.

### Parameters

-   **targetNode**

    The target node on which to perform the clean operation.


### Returns

void

### Example

```

          siteService.cleanSitePermissions(node);
      
```

## `cleanSitePermissions(NodeRef targetNode)`

`cleanSitePermissions(NodeRef targetNode)` cleans permissions from the node specified by the supplied nodeRef.

### Parameters

-   **targetNode**

    The node reference of the target node on which to perform the clean operation.


### Returns

void

### Example

```

          siteService.cleanSitePermissions(nodeRef);
      
```

