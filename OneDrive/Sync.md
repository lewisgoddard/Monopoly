## Configure Sync Settings in Microsoft OneDrive

### Silently sign in users to the OneDrive sync app with their Windows credentials

If you enable this setting, users who are signed in on a PC that's joined to Azure AD can set up the sync app without entering their account credentials. Users will still be shown OneDrive Setup so they can select folders to sync and change the location of their OneDrive folder.

- GP unique name: **[SilentAccountConfig](https://docs.microsoft.com/en-us/onedrive/use-group-policy#silently-sign-in-users-to-the-onedrive-sync-app-with-their-windows-credentials)**
- GP name: Silently sign in users to the OneDrive sync app with their Windows credentials
- GP path (Mandatory): **Computer Configuration\Policies\Administrative Templates\OneDrive**
- GP path (Recommended): N/A
- GP ADMX file name: `OneDrive.admx`

### [Silently move Windows known folders to OneDrive](https://docs.microsoft.com/en-us/onedrive/use-group-policy#silently-move-windows-known-folders-to-onedrive)

_Note: Microsoft recommend deploying the silent policy for existing devices and new devices while limiting the deployment of existing devices to 1,000 devices a day and not exceeding 4,000 devices a week. Microsoft also recommend using this setting together with "Prompt users to move Windows known folders to OneDrive." If moving the known folders silently does not succeed, users will be prompted to correct the error and continue._

#### Options

**Computer Configuration\Policies\Administrative Templates\OneDrive**
- Tennant ID like 1111-2222-3333-4444
- Show Notification: 0. No, 1. Yes

If you don't set any of the following policies then the default policy will move all the folders (Desktop, Documents and Pictures) into OneDrive. If you want to specify which folder(s) to move then you can set any combination of the following options on this policy:

- KFMSilentOptInDesktop
- KFMSilentOptInDocuments
- KFMSilentOptInPictures

### [Prompt users to move Windows known folders to OneDrive](https://docs.microsoft.com/en-us/onedrive/use-group-policy#prompt-users-to-move-windows-known-folders-to-onedrive)

_Note: Microsoft recommend deploying the prompt policy for existing devices only, and limiting the deployment to 5,000 devices a day and not exceeding 20,000 devices a week._

If you enable this setting and provide your tenant ID, users who are syncing their OneDrive see the previous window when they're signed in. If they close the window, a reminder notification appears in the Activity Center until they move all their known folders. If a user has already redirected their known folders to a different OneDrive account, they are prompted to direct the folders to the account for your organization (leaving existing files behind).

If you disable or do not configure this setting, the window that prompts users to protect their important folders doesn't appear.

- **Computer Configuration\Policies\Administrative Templates\OneDrive\KFMOptInWithWizard**

### References
- https://docs.microsoft.com/en-us/onedrive/use-group-policy#silently-sign-in-users-to-the-onedrive-sync-app-with-their-windows-credentials
- https://docs.microsoft.com/en-us/onedrive/use-silent-account-configuration
- https://docs.microsoft.com/en-us/onedrive/redirect-known-folders
- https://docs.microsoft.com/en-us/onedrive/use-group-policy#silently-move-windows-known-folders-to-onedrive
- https://docs.microsoft.com/en-us/onedrive/use-group-policy#prompt-users-to-move-windows-known-folders-to-onedrive
