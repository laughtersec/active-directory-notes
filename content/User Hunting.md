---
publish: true
created: 2025-02-23T23:53:09.704+05:30
modified: 2025-12-06T16:15:14.952+05:30
published: 2025-12-06T16:15:14.952+05:30
tags:
  - domain-enumeration
cssclasses: []
---

```powershell title:"Find all machines on the current domain where the current user has local admin access"
Find-LocalAdminAccess -Verbose
```

This function queries the DC of the current or provided domain for a list of computers (`Get-NetComputer`) and then use multi-threaded `Invoke-CheckLocalAdminAccess` on each machine.

This can also be done with the help of remote administration tools like WMI and PowerShell remoting. Pretty useful in cases ports (RPC and SMB) used by `Find-LocalAdminAccess` are blocked. See `Find-WMILocalAdminAccess.ps1` and `Find-PSRemotingLocalAdminAccess.ps1`

```powershell title:"Find computers where a domain admin (or specified user/group) has sessions:"
1. Find-DomainUserLocation -Verbose
2. Find-DomainUserLocation -UserGroupIdentity "RDPUsers"
```

This function queries the DC of the current or provided domain for members of the given group (Domain Admins by default) using `Get-DomainGroupMember`, gets a list of computers (`Get-DomainComputer`) and list sessions and logged on users (`Get-NetSession/Get-NetLoggedon`) from each machine.

_Note that Server 2019 onwards, local administrator privileges are required to list sessions._

```powershell title:"Find computers where a domain admin session is available and current user has admin access (uses Test-AdminAccess)"
Find-DomainUserLocation -CheckAccess
```

```powershell title:"Find computers (File Servers and Distributed File servers) where a domain admin session is available."
Find-DomainUserLocation -Stealth
```

```powershell title:"List sessions on remote machines (Not PowerView)"
Invoke-SessionHunter -FailSafe
```

_Above command doesn't need admin access on remote machines. Uses Remote Registry and queries HKEY\_USERS hive._

```powershell title:"Opsec friendly command (Not PowerView)"
Invoke-SessionHunter -NoPortScan -Targets C:\Path\To\servers.txt
```

An over-reliance on automated tools is not the wisest choice.

We can find domain users from our current foothold too.

```shell title:"Find domain users"
net user /domain
```

We can fetch its details too

```shell title:"List details of a domain user"
net user "domain.user" /domain
```
