## Configure Space Settings in Microsoft OneDrive

### Use OneDrive Files On-Demand

**Computer Configuration\Policies\Administrative Templates\OneDrive**

If you enable this setting, new users who set up the sync app see online-only files in File Explorer, by default. File contents don't download until a file is opened.

If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.

If you do not configure this setting, users can turn Files On-Demand on or off.

### Block file downloads when users are low on disk space

This setting lets you specify a minimum amount of available disk space and block OneDrive from downloading files when users have less than this amount.

Users are prompted with options to help free up space.

_Setting is in MB, with accepted values from 0 through 10,240,000. Default value is 200 MB._

### Warn users who are low on disk space

**Computer Configuration\Policies\Administrative Templates\OneDrive**

This setting lets you specify a minimum amount of available disk space, and warn users when the OneDrive sync app downloads a file that causes them to have less than this amount. Users are prompted with options to help free up space.

_Setting is in MB, with accepted values from 0 through 10,240,000. Default value is 500 MB._

### Set the maximum size of a user's OneDrive that can download automatically

_Note: This setting is only used with Silently sign in users to OneDrive with their Windows credentials on devices that don't have OneDrive Files On-Demand enabled._

Any user who has a OneDrive that's larger than the specified threshold (in MB) is prompted to choose the folders they want to sync before OneDrive downloads the files.

_Setting is in MB, with accepted values from 0 through 4,294,967,295. There is no default value,a dn you will require your Tenant ID._

### References
- https://docs.microsoft.com/en-us/onedrive/use-group-policy#use-onedrive-files-on-demand
- https://admx.help/?Category=OneDrive&Policy=Microsoft.Policies.OneDriveNGSC::FilesOnDemandEnabled
- https://docs.microsoft.com/en-us/onedrive/use-group-policy#warn-users-who-are-low-on-disk-space
- https://admx.help/?Category=OneDrive&Policy=Microsoft.Policies.OneDriveNGSC::WarningMinDiskSpaceLimitInMB
- https://docs.microsoft.com/en-us/onedrive/use-group-policy#set-the-maximum-size-of-a-users-onedrive-that-can-download-automatically
- https://admx.help/?Category=OneDrive&Policy=Microsoft.Policies.OneDriveNGSC::DiskSpaceCheckThresholdMB
- https://docs.microsoft.com/en-us/onedrive/use-group-policy#block-file-downloads-when-users-are-low-on-disk-space
