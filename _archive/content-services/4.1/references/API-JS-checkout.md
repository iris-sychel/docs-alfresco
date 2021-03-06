---
author: [Alfresco Documentation, Alfresco Documentation]
source: JavaScript API
audience: 
category: JS API
option: checkout
---

# `checkout`

The checkout methods perform checkouts of versionable nodes.

**Parent topic:**[Check In/Check Out API](../references/API-JS-CheckInOut.md)

## `checkout ()`

`checkout()` this method performs a checkout of the node.

### Returns

Returns the resulting working copy node.

### Example

```

    var workingCopy;
    var node = companyhome.childByNamePath("TEST_FILE_1.TXT");

    node.ensureVersioningEnabled(true, true);
    
    if (node.isVersioned){
        
        workingCopy = node.checkout();
        workingCopy.content = "Add some content.";
        workingCopy.checkin("Added some content.");
    }

        
```

## ``checkout(destination)``

`checkout(destination)` this method performs a check out of the node to the specified destination.

### Returns

Returns the resulting working copy node.

