---
publish: true
created: 2025-02-23T23:53:09.696+05:30
modified: 2025-08-15T16:41:51.629+05:30
published: 2025-08-15T16:41:51.629+05:30
tags:
  - detection-and-defense
cssclasses: []
---

- [Credential Guard](https://learn.microsoft.com/en-us/windows/security/identity-protection/credential-guard/) uses virtualization-based security to isolate secrets so that only privileged system software can access them.
- Effective in stopping PTH and Over-PTH attacks by restricting access to NTLM hashes and TGTs. It is not possible to write Kerberos tickets to memory even if we have credentials.
- However, credentials for local accounts in SAM and Service Account credentials from LSA Secrets are **not** protected.
- Credential Guard cannot be enabled on a DC as it breaks authentication there.
- Only available on Windows 10+ Enterprise edition and Server 2016 or later.
- Mimikatz can bypass it.
