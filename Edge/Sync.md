# Configure Sync Settings in Microsoft Edge

### Automatic Sign-in

If your device is hybrid-domain-joined, the user gets automatically signed in with their Azure AD account.

_No configuration is necessary._ [[1](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-security-identity#automatic-sign-in)]

You can use the `BrowserSignin` policy [[2](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#browsersignin)] to force users to sign in before use,  
but this seems likely to cause friction so we do not advise it.

### Auto-Configure Sync

Forces data synchronization in Microsoft Edge, bypassing consent prompt.  
This policy also prevents the user from turning sync off.

0 = Do not automatically start sync and show the sync consent (default)  
1 = Force sync to be turned on for Azure AD/Azure AD-Degraded user profile and do not show the sync consent prompt

- GP unique name: **ForceSync**
- GP name: Force synchronization of browser data and do not show the sync consent prompt
- GP path (Mandatory): **Administrative Templates/Microsoft Edge/**
- GP path (Recommended): N/A
- GP ADMX file name: `MSEdge.admx`

#### References
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-security-identity#automatic-sign-in
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#browsersignin
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#forcesync
