---
publish: true
created: 2025-02-23T23:53:09.699+05:30
modified: 2025-08-15T16:42:13.389+05:30
published: 2025-08-15T16:42:13.389+05:30
tags:
  - general
aliases:
cssclasses:
---

![[Kerberos.svg]]

1. AS-REQ: Time stamp encrypted with NTLM hash to request for a signed TGT is sent to the Key Distribution Center (KDC) on the DC.
2. AS-REP: Initial request is encrypted with the krbtgt account hash and sent back to the client in the form of a Ticket-Granting-Ticket
3. TGS-REQ: The TGT is sent to the KDC to request a Ticket Granting Service ticket
4. TGS-REP: The TGT is encrypted with the service account's hash and sent back to the client in the form of a TGS
5. AP-REQ:
