---
publish: true
created: 2025-02-23T23:53:09.697+05:30
modified: 2025-08-15T16:42:09.386+05:30
published: 2025-08-15T16:42:09.386+05:30
tags:
  - detection-and-defense
cssclasses:
---

## Enhanced Security Admin Environment

![[ESAE.svg]]

- Dedicated administrative forest for managing critical assets like administrative users, groups and computers.
- Since a forest is considered a security boundary rather than a domain, this model provides enhanced security controls.
- The administrative forest is also called the Red Forest.
- Administrative users in a production forest are used as standard non-privileged users in the administrative forest.
- Selective Authentication to the Red Forest enables stricter security controls on logon of users from non-administrative forests.
- Microsoft retired ESAE in 2021 and replaced it with Privileged Access Strategy.
