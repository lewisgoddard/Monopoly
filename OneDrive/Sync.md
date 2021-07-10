## Configure Sync Settings in Microsoft OneDrive

### Silently sign in users to the OneDrive sync app with their Windows credentials

If you enable this setting, users who are signed in on a PC that's joined to Azure AD can set up the sync app without entering their account credentials. Users will still be shown OneDrive Setup so they can select folders to sync and change the location of their OneDrive folder.

- GP unique name: **[SilentAccountConfig](https://docs.microsoft.com/en-us/onedrive/use-group-policy#silently-sign-in-users-to-the-onedrive-sync-app-with-their-windows-credentials)**
- GP name: Silently sign in users to the OneDrive sync app with their Windows credentials
- GP path (Mandatory): **Computer Configuration\Policies\Administrative Templates\OneDrive**
- GP path (Recommended): N/A
- GP ADMX file name: `OneDrive.admx`

### References
- https://docs.microsoft.com/en-us/onedrive/use-group-policy#silently-sign-in-users-to-the-onedrive-sync-app-with-their-windows-credentials
- https://docs.microsoft.com/en-us/onedrive/use-silent-account-configuration
