## Configure Sync Settings in Microsoft Edge

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

## Configure Password Settings in Microsoft Edge

### Allow user to Save Passwords

Enable Microsoft Edge to save user passwords.

If you enable this policy, users can save their passwords in Microsoft Edge.  
The next time they visit the site, Microsoft Edge will enter the password automatically.

If you disable this policy, users can't save new passwords, but they can still use previously saved passwords.

- GP unique name: **PasswordManagerEnabled**
- GP name: Enable saving passwords to the password manager
- GP path (Mandatory): **Administrative Templates/Microsoft Edge/Password manager and protection**
- GP path (Recommended): **Administrative Templates/Microsoft Edge - Default Settings (users can override)/Password manager and protection**
- GP ADMX file name: `MSEdge.admx`

### Monitor Users Saved Passwords

Allow users to be alerted if their passwords are found to be unsafe

If you enable this policy and a user consents to enabling the policy, the user will get alerted if any of their passwords stored in Microsoft Edge are found to be unsafe. Microsoft Edge will show an alert and this information will also be available in **Settings > Passwords > Password Monitor**.

If you disable this policy, users will not be asked for permission to enable this feature. Their passwords will not be scanned and they will not be alerted either.

If you enable or don't configure the policy, users can turn this feature on or off.

To learn more about how Microsoft Edge finds unsafe passwords see https://go.microsoft.com/fwlink/?linkid=2133833

**Special guidance:**

Settings the policy as mandatory results in the policy error message: "This policy value is ignored because Password Monitor requires the consent of the individual user for it to be turned on. You can ask users in your Organization to go to Settings > Profile > Password and turn on the feature."

- GP unique name: **PasswordMonitorAllowed**
- GP name: Allow users to be alerted if their passwords are found to be unsafe
- GP path (Mandatory): Do NOT set, see special guidance.
- GP path (Recommended): **Administrative Templates/Microsoft Edge - Default Settings (users can override)/Password manager and protection**
- GP ADMX file name: `MSEdge.admx`

### References
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-security-identity#automatic-sign-in
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#browsersignin
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#forcesync
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#passwordmanagerenabled
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#passwordmonitorallowed
- https://go.microsoft.com/fwlink/?linkid=2133833
