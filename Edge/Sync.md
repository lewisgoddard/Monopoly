### Automatic Sign-in
Depending on how a device is configured, users can get auto signed into Microsoft Edge using one of the following approaches.

- **The device is hybrid/AAD-J**: Available on Win10, down-level Windows, and corresponding server versions. The user gets automatically signed in with their Azure AD account.
- **The device is domain joined**: Available on Win10, down-level Windows, and corresponding server versions. By default, the user will not get automatically signed in. If you want to automatically sign in users with domain accounts, use the ConfigureOnPremisesAccountAutoSignIn policy. If you want to automatically sign in users with their Azure AD accounts, consider hybrid joining your devices.
- **OS default account is MSA**: Win10 RS3 (Version 1709/Build 10.0.16299) and above. This scenario is unlikely on enterprise devices. But, if the OS default account is MSA, Microsoft Edge will sign in automatically with the MSA account.
