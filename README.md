# Monopoly

Configuration items for full Microsoft integration with online services from a hybrid domain systems.

## Supported Products

- [Edge](Edge)
- OneDrive
- Sharepoint
- Office
- Teams
- Defender

## ADMX Sources

Edge: https://www.microsoft.com/en-us/edge/business/download  
Windows 10 (and 8.1): https://docs.microsoft.com/en-us/troubleshoot/windows-client/group-policy/create-and-manage-central-store

## Assumptions

### OU Structure

- Employees
    - Accounts
    - Sales
- Workstations
    - Accounts
    - Sales
- IT
    - Accounts
    - Admin Accounts
    - Workstations
- Servers
  - Hypervisors
  - Virtual Machines
      - Exchange Servers
      - Other VMs
      - SQL Servers
