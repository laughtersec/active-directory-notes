---
publish: true
created: 2025-02-23T23:53:09.703+05:30
modified: 2025-08-15T16:43:37.014+05:30
published: 2025-08-15T16:43:37.014+05:30
tags:
  - detection-and-defense
---

#### Active Directory Administrative Tier Model

- Composed of three levels only for administrative accounts:
  - Tier 0 - Accounts, Groups and Computers which have privileges across the enterprise like Domain Controllers, Domain Admins, Enterprise Admins.
  - Tier 1 - Accounts, Groups and Computers which have access to resources having significant amount of business value. A common example role is server administrators who maintain these operating systems with the ability to impact all enterprise services.
  - Tier 2 - Administrator accounts which have administrative control of a significant amount of business value that is hosted on user workstations and devices. Examples include Help Desk and computer support administrators because they can impact the integrity of almost any user data.
- Control Restrictions - What admins control
- Logon Restrictions - Where admins can log-on to
