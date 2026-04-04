---
publish: true
created: 2025-02-23T23:53:09.694+05:30
modified: 2025-04-04T22:07:48.710+05:30
published: 2025-04-04T22:07:48.710+05:30
tags:
  - general
cssclasses:
---

#### [Access Control Model](https://learn.microsoft.com/en-us/windows/win32/secauthz/access-control-model)

Enables control on the ability of a process to access objects and other resources in windows based on:

- Access Tokens (security context of a process - identity of privileges of the user)
- Security Descriptors (SID of the owner, Discretionary ACL (DACL) and System ACL (SACL))

#### SID Diagram

![[SID.svg]]

#### Access Control List (ACL)

![[png/accctrl1.png]]

- It is a list of Access Control Entries (ACE) - ACE corresponds to individual permission or audit access. It helps determining who has permissions and what can be done on an object. There are two types of ACLs:
  - Discretionary Access Control List (DACL) - Defines the permissions trustees (a user or group) have on an object.
  - System Access Control List (SACL) - Logs success and failure audit messages when an object is accessed.
- ACLs are vital to security architecture of AD
- The order of the ACEs is important because the system reads the ACEs in sequence until access is granted or denied.
- A null or empty DACL grants full access to any user that requests it. An empty DACL is properly allocated and initialized with no ACEs, and is not the same as a null DACL.
