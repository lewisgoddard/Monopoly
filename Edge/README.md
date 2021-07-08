## Configure Microsoft Edge

### Prepare to Configure Microsoft Edge

1. Download Policy Files from https://www.microsoft.com/en-us/edge/business/download
    - `msedge.admx` to configure Microsoft Edge settings
    - `msedgeupdate.admx` to manage Microsoft Edge updates.
2. Copy to Active Directory https://docs.microsoft.com/en-us/deployedge/configure-microsoft-edge#add-the-administrative-template-to-active-directory

### Test Configuration of Microsoft Edge

1. Run `gpupdate /force`
2. Visit `edge://policy` in Microsoft Edge

### References

- [Add the Administrative Template to Active Directory](https://docs.microsoft.com/en-us/deployedge/configure-microsoft-edge#add-the-administrative-template-to-active-directory)
- [Test Your Policies](https://docs.microsoft.com/en-us/deployedge/configure-microsoft-edge#3-test-your-policies)
