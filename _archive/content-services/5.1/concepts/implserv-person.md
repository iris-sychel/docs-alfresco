---
author: [Alfresco Documentation, Alfresco Documentation]
source: Professional Alfresco Book
audience: 
category: [Authentication and Security, Security, Developer]
keyword: [Person service, security]
---

# Person service

Use this information to understand and configure of person service.

The `PersonService` interface is the API by which nodes of the person type, as defined in [contentModel.xml](http://dev.alfresco.com/resource/AlfrescoOne/5.0/configuration/alfresco/model/contentModel.xml), should be accessed.

The `PersonService` is responsible for all of the following:

-   Obtaining a reference to the Person node for a given user name
-   Determining if a person entry exists for a user
-   Potentially creating missing people entries with default settings on demand
-   Supplying a list of mutable properties for each person
-   Creating, deleting, and altering personal information

The beans to support the `PersonService` and its configuration can be found in [authentication-services-context.xml](http://dev.alfresco.com/resource/AlfrescoOne/5.0/configuration/alfresco/authentication-services-context.xml). The principle configuration options are around how people are created on demand if users are managed by using NTLM or some other external user repository.

**Parent topic:**[Implementation and services](../concepts/secur-implserv.md)

