---
{"publish":true,"created":"2025-02-23T23:53:09.703+05:30","modified":"2025-08-15T16:43:37.895+05:30","published":"2025-08-15T16:43:37.895+05:30","tags":["defense"],"cssclasses":""}
---

#### JIT
- Just In Time administration provides the ability to grant time-bound administrative access on per-request basis.
- Check out Temporary Group Membership (Requires Privileged Access Management Feature to be enabled which can't be turned off later)

```powershell
Add-ADGroupMember -Identity 'Domain Admins' -Members newDA -MemberTimeToLive (New-TimeSpan -Minutes 60)
```

#### JEA
- Just Enough Administration provides role based access control for PowerShell based remote delegated administration.
- With JEA non-admin users can connect remotely to machines for doing specific administrative tasks.
- For instance, we can control the command a user can run and even restrict parameters which can be used.
- JEA endpoints have PowerShell transcription and logging enabled.