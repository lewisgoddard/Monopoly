## Configure Microsoft Edge Security Settings

### Configure Automatic HTTPS

This feature helps protect against man-in-the-middle attacks by enforcing more secure connections, but users might experience more connection errors.

#### Policy options mapping:

DisableAutomaticHttps (0) = Automatic HTTPS functionality is disabled.

UpgradeCapableDomains (1) [Default] = Navigations delivered over HTTP are switched to HTTPS, only on domains likely to support HTTPS.

AlwaysUpgrade (2) = All navigations delivered over HTTP are switched to HTTPS. Connection errors might occur more often.

_Note: The 'UpgradeCapableDomains' configuration requires a component list, and will not upgrade these connections if ComponentUpdatesEnabled is set to 'Disabled'._

Use the preceding information when configuring this policy.

- GP unique name: **AutomaticHttpsDefault**
- GP name: Configure Automatic HTTPS
- GP path (Mandatory): **Administrative Templates/Microsoft Edge/**
- GP path (Recommended): **Administrative Templates/Microsoft Edge - Default Settings (users can override)/**
- GP ADMX file name: `MSEdge.admx`

### Configure Microsoft Defender SmartScreen

This policy setting lets you configure whether to turn on Microsoft Defender SmartScreen. Microsoft Defender SmartScreen provides warning messages to help protect your users from potential phishing scams and malicious software. _By default, Microsoft Defender SmartScreen is turned on._

If you enable this setting, Microsoft Defender SmartScreen is turned on.

If you disable this setting, Microsoft Defender SmartScreen is turned off.

_If you don't configure this setting, users can choose whether to use Microsoft Defender SmartScreen._

- GP unique name: **SmartScreenEnabled**
- GP name: Configure Microsoft Defender SmartScreen
- GP path (Mandatory): **Administrative Templates/Microsoft Edge/SmartScreen settings**
- GP path (Recommended): **Administrative Templates/Microsoft Edge - Default Settings (users can override)/SmartScreen settings**
- GP ADMX file name: `MSEdge.admx`

### Prevent bypassing Microsoft Defender SmartScreen prompts for sites

This policy setting lets you decide whether users can override the Microsoft Defender SmartScreen warnings about potentially malicious websites.

If you enable this setting, users can't ignore Microsoft Defender SmartScreen warnings and they are blocked from continuing to the site.

If you disable or don't configure this setting, users can ignore Microsoft Defender SmartScreen warnings and continue to the site.

- GP unique name: **PreventSmartScreenPromptOverride**
- GP name: Prevent bypassing Microsoft Defender SmartScreen prompts for sites
- GP path (Mandatory): **Administrative Templates/Microsoft Edge/SmartScreen settings**
- GP path (Recommended): N/A
- GP ADMX file name: `MSEdge.admx`

### Prevent bypassing Microsoft Defender SmartScreen warnings about downloads

This policy lets you determine whether users can override Microsoft Defender SmartScreen warnings about unverified downloads.

If you enable this policy, users in your organization can't ignore Microsoft Defender SmartScreen warnings, and they're prevented from completing the unverified downloads.

If you disable or don't configure this policy, users can ignore Microsoft Defender SmartScreen warnings and complete unverified downloads.

- GP unique name: **PreventSmartScreenPromptOverrideForFiles**
- GP name: Prevent bypassing of Microsoft Defender SmartScreen warnings about downloads
- GP path (Mandatory): **Administrative Templates/Microsoft Edge/SmartScreen settings**
- GP path (Recommended): N/A
- GP ADMX file name: `MSEdge.admx`

### Configure Microsoft Defender SmartScreen to block potentially unwanted apps

This policy setting lets you configure whether to turn on blocking for potentially unwanted apps with Microsoft Defender SmartScreen. Potentially unwanted app blocking with Microsoft Defender SmartScreen provides warning messages to help protect users from adware, coin miners, bundleware, and other low-reputation apps that are hosted by websites. Potentially unwanted app blocking with Microsoft Defender SmartScreen is turned off by default.

If you enable this setting, potentially unwanted app blocking with Microsoft Defender SmartScreen is turned on.

If you disable this setting, potentially unwanted app blocking with Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use potentially unwanted app blocking with Microsoft Defender SmartScreen.

- GP unique name: **SmartScreenPuaEnabled**
- GP name: Configure Microsoft Defender SmartScreen to block potentially unwanted apps
- GP path (Mandatory): **Administrative Templates/Microsoft Edge/SmartScreen settings**
- GP path (Recommended): **Administrative Templates/Microsoft Edge - Default Settings (users can override)/SmartScreen settings**
- GP ADMX file name: `MSEdge.admx`

### See also
- [Microsoft Security Compliance Toolkit](https://www.microsoft.com/en-us/download/details.aspx?id=55319)

### References
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#configure-automatic-https
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#smartscreenenabled
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#preventsmartscreenpromptoverride
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#preventsmartscreenpromptoverrideforfiles
- https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#smartscreenpuaenabled
