## Configure Microsoft Internet Explorer

The Internet Explorer 11 desktop application will be retired and go out of support on **June 15th, 2022** (for a list of what’s in scope, [see the FAQ](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/internet-explorer-11-desktop-app-retirement-faq/ba-p/2366549)). The same IE11 apps and sites you use today can open in Microsoft Edge with Internet Explorer mode. [Learn more here](https://blogs.windows.com/windowsexperience/2021/05/19/the-future-of-internet-explorer-on-windows-10-is-in-microsoft-edge/).

To disable Internet Explorer 11 using group policy, follow these steps:

### Prepare to Configure Microsoft Internet Explorer: Prerequisite Updates

1. Ensure you have the pre-requisite operating system updates. This step will update the ADMX files on your machine directly (specifically `inetres.adml` and `inetres.admx`). Please note that if you want to update your Central Store, you will need to copy over the .adml and .admx files from a machine that has the pre-requisite updates.

- Windows updates
  - Windows 10, version 2004, Windows Server version 2004, Windows 10, version 20H2: KB4598291 or later
  - Windows 10 version 1909, Windows Server version 1909: KB4598298 or later
  - Windows 10 version 1809, Windows Server version 1809, and Windows Server 2019: KB4598296 or later
  - Windows 10, version 1607, Windows Server 2016: KB4601318 or later
  - Windows 10 initial version (July 2015): KB4601331 or later
  - Windows 8.1: KB4601384 or later
  - Windows Server 2012: KB4601348 or later
- Microsoft Edge Stable Channel

### Disable Microsoft Internet Explorer

2. Go to **Computer Configuration/Administrative Templates/Windows Components/Internet Explorer**

3. Double-click **Disable Internet Explorer 11 as a standalone browser**

4. Select **Enabled**

5. Under **Options**, pick one of the following values:

    - Never if you don’t want to notify users that IE11 is disabled.
    - Always if you want to notify users every time they're redirected from IE11.
    - Once per user if you want to notify users only the first time they are redirected.
 
6. Click OK or Apply to save this policy setting.

### References

- [Disable Internet Explorer 11](https://docs.microsoft.com/en-us/deployedge/edge-ie-disable-ie11)
