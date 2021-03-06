---
author: Alfresco Documentation
---

# Versions API

The Versions ScriptNode API provides several methods and properties for managing and retrieving the versions of a document.

## Properties

-   **`isVersioned`**

    A read-only Boolean property for determining if the document is versioned.

-   **`versionHistory`**

    A read-only property for listing all versions of the document in descending \(version created\) date order.


-   **[Script Version Object](../references/API-JS-ScriptVersion.md)**  
The Versions ScriptNode API provides methods that return `ScriptVersion` objects, for example, `getVersion()`. ScriptVersion objects have the following properties.
-   **[getVersion](../references/API-JS-getVersion.md)**  
`getVersion(label)` gets a specific version of a document identified by `label`.
-   **[createVersion](../references/API-JS-createVersion.md)**  
`createVersion(history, major)` this method creates a version snapshot of the current document.
-   **[ensureVersioningEnabled](../references/API-JS-ensureVersioningEnabled.md)**  
 `ensureVersioningEnabled(autoVersion, autoVersionProps)` ensures that this node has the `cm:versionable` aspect applied to it, and that it has the initial version in the version store.
-   **[getVersionHistory](../references/API-JS-getVersionHistory.md)**  
 `getVersionHistory()` gets the version history for the current node.

**Parent topic:**[ScriptNode API](../references/API-JS-ScriptNode.md)

