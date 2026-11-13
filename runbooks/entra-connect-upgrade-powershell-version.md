# Entra Connect upgrade failed because of PowerShell 7

| | |
| --- | --- |
| **Area** | Entra Connect (hybrid identity) |
| **Date** | [FILL IN: month and year] |
| **Impact** | Upgrade blocked; [FILL IN: was directory sync affected while it was blocked?] |

## Symptom

The Entra Connect upgrade failed partway through.

[FILL IN: the exact error text from the installer or its log]

## Environment

- Windows Server 2019, on-premises Active Directory synced to Entra ID with Entra Connect
- Both Windows PowerShell 5.1 and PowerShell 7 installed on the server
- [FILL IN: Entra Connect version before and after]

## Cause

The upgrade ran against PowerShell 7 where it needed Windows PowerShell 5.1.

[FILL IN: the specific mechanism. For example, which module or command failed under PowerShell 7, and how you traced it: installer log location, the line that pointed to the version mismatch]

## Fix

1. [FILL IN: what you changed so the upgrade used Windows PowerShell 5.1]
2. [FILL IN: how you re-ran the upgrade]

## Verify

- [FILL IN: version shown after upgrade]
- [FILL IN: how you confirmed sync was healthy, e.g. a successful delta sync cycle and no errors in the sync service]

## Prevention

- [FILL IN: e.g. a pre-upgrade check added to the runbook for this server]

## References

- [FILL IN: Microsoft documentation used]
