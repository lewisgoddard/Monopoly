# Monopoly

Configuration items for full Microsoft integration with online services from a hybrid domain systems.

## Supported Products

- Microsoft Defender
- [Microsoft Edge](Edge)
- Microsoft Office
- Microsoft OneDrive
- Microsoft Sharepoint
- Microsoft Teams
- Microsoft Windows

_Note: Microsoft Defender Smartscreen has some configuration items within Microsoft Edge._

## ADMX Sources

Edge: https://www.microsoft.com/en-us/edge/business/download  
Internet Explorer: Bundled with Windows 10  
Windows 10 (and 8.1): https://docs.microsoft.com/en-us/troubleshoot/windows-client/group-policy/create-and-manage-central-store  

## Assumptions

### OU Structure

- Employees
    - Accounts
    - IT
    - Sales
- Workstations
    - Accounts
    - IT
    - Sales
- IT
    - Admin Accounts
    - Admin Workstations
- Servers
  - Hypervisors
  - Virtual Machines
      - Exchange Servers
      - Other VMs
      - SQL Servers
