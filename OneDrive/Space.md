## Configure Space Settings in Microsoft OneDrive

### [Use OneDrive Files On-Demand](https://docs.microsoft.com/en-us/onedrive/use-group-policy#use-onedrive-files-on-demand)

If you enable this setting, new users who set up the sync app see online-only files in File Explorer, by default. File contents don't download until a file is opened. If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand. If you do not configure this setting, users can turn Files On-Demand on or off.

- GP unique name: **FilesOnDemandEnabled**
- GP name: Enable OneDrive Files On-Demand
- GP path (Mandatory): **Computer Configuration\Policies\Administrative Templates\OneDrive**
- GP path (Recommended): N/A
- GP ADMX file name: `OneDrive.admx`

### [Warn users who are low on disk space](https://docs.microsoft.com/en-us/onedrive/use-group-policy#warn-users-who-are-low-on-disk-space)

This setting lets you specify a minimum amount of available disk space, and warn users when the OneDrive sync app downloads a file that causes them to have less than this amount. Users are prompted with options to help free up space.

Setting is in MB, with accepted values from 0 through 10,240,000. Default value is 500 MB.

- GP unique name: **WarningMinDiskSpaceLimitInMB**
- GP name: Warn users who are low on disk space
- GP path (Mandatory): **Computer Configuration\Policies\Administrative Templates\OneDrive**
- GP path (Recommended): N/A
- GP ADMX file name: `OneDrive.admx`

### References
- https://docs.microsoft.com/en-us/onedrive/use-group-policy#use-onedrive-files-on-demand
- https://docs.microsoft.com/en-us/onedrive/use-group-policy#warn-users-who-are-low-on-disk-space
- https://admx.help/?Category=OneDrive&Policy=Microsoft.Policies.OneDriveNGSC::WarningMinDiskSpaceLimitInMB
