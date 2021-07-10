## Configure Microsoft Edge Security Settings

These settings are based on the [Microsoft Security Compliance Toolkit](https://www.microsoft.com/en-us/download/details.aspx?id=55319) for Edge 88.

| Unique | Description | Microsoft Baseline | Policy Default | Monopoly Recommends |
|--------|-------------|--------------------|----------------|---------------------|
| [SitePerProcess](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#siteperprocess) | Enable site isolation for every site | Enabled | **User choice** | Enabled |
| [SmartScreenEnabled](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#smartscreenenabled) | Configure Microsoft Defender SmartScreen | Enabled | **User choice** | Enabled |
| [SmartScreenPuaEnabled](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#smartscreenpuaenabled) | Configure Microsoft Defender SmartScreen to block potentially unwanted apps | Enabled | **User choice** | Enabled |
| [PreventSmartScreenPromptOverride](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#preventsmartscreenpromptoverride) | Prevent bypassing Microsoft Defender SmartScreen prompts for sites | Enabled | **User choice** | Enabled |
| [PreventSmartScreenPromptOverrideForFiles](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#preventsmartscreenpromptoverrideforfiles) | Prevent bypassing of Microsoft Defender SmartScreen warnings about downloads | Enabled | **User choice** | Enabled |
| [NativeMessagingUserLevelHosts](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#nativemessaginguserlevelhosts) | Allow user-level native messaging hosts (installed without admin permissions) | Disabled | **Enabled** | Disabled
| [AuthSchemes](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#authschemes) | Supported authentication schemes | ntlm, negotiate | **basic, digest, ntlm, negotiate** | _Depends_ |
| [BasicAuthOverHttpEnabled](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#basicauthoverhttpenabled) | Allow Basic authentication for HTTP | Disabled | **Enabled** | _Depends_ |
| [SSLErrorOverrideAllowed](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#sslerroroverrideallowed) | Allow users to proceed from the HTTPS warning page | Disabled | **Enabled** | _Depends_ |
| [ExtensionInstallBlocklist](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#extensioninstallblocklist) | Control which extensions cannot be installed | Enabled: * | **Disabled** | _Depends_ |
| [PasswordManagerEnabled](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#passwordmanagerenabled) | Enable saving passwords to the password manager | Disabled | **User choice** | Enabled |
| [SSLVersionMin](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#sslversionmin) | Minimum TLS version enabled (**Deprecated**) | Hard Enabled: TLS 1.2 | **Soft Enabled: TLS 1.2** | _Deprecated_ |
| [DefaultPluginsSetting](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#defaultpluginssetting) | Default Adobe Flash setting (**Obsolete**) | Enabled: (2) Block the Adobe Flash plugin | **User choice** | _Obsolete_ |
| [EnableSha1ForLocalAnchors](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies#enablesha1forlocalanchors) | Allow certificates signed using SHA-1 when issued by local trust anchors (**Obsolete**) | Disabled | Disabled | _Obsolete_ |
