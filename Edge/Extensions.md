## Configure Microsoft Edge Extension Settings

### Block External Extensions

- GP unique name: **BlockExternalExtensions**
- GP name: Blocks external extensions from being installed
- GP path (Mandatory): **Administrative Templates/Microsoft Edge/Extensions**
- GP path (Recommended): N/A
- GP ADMX file name: `MSEdge.admx`

### Block All Extensions

Lets you specify which extensions the users CANNOT install. Extensions already installed will be disabled if blocked, without a way for the user to enable them. After a disabled extension is removed from the blocklist it will automatically get re-enabled.

A blocklist value of '*' means all extensions are blocked unless they are explicitly listed in the allowlist.

If this policy isn't set, the user can install any extension in Microsoft Edge.

- GP unique name: **ExtensionInstallBlocklist**
- GP name: Control which extensions cannot be installed
- GP path (Mandatory): **Administrative Templates/Microsoft Edge/Extensions**
- GP path (Recommended): N/A
- GP ADMX file name: `MSEdge.admx`

### Automatically Install Extensions

Set this policy to specify a list of apps and extensions that install silently, without user interaction. Users can't uninstall or turn off this setting. Permissions are granted implicitly, including the enterprise.deviceAttributes and enterprise.platformKeys extension APIs. Note: These 2 APIs aren't available to apps and extensions that aren't force-installed.

If you don't set this policy, no apps or extensions are autoinstalled and users can uninstall any app in Microsoft Edge.

This policy supercedes **ExtensionInstallBlocklist** policy. If a previously force-installed app or extension is removed from this list, Microsoft Edge automatically uninstalls it.

_Note: This policy doesn't apply to InPrivate mode._

- GP unique name: **ExtensionInstallForcelist**
- GP name: Control which extensions are installed silently
- GP path (Mandatory): **Administrative Templates/Microsoft Edge/Extensions**
- GP path (Recommended): N/A
- GP ADMX file name: `MSEdge.admx`

### References
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#blockexternalextensions
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#extensioninstallblocklist
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#extensioninstallforcelist
