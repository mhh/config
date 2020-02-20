# Windows installation
1. Download a Windows 10 Enterprise edition image from [Visual Studio Subscriptions][vss-windows]
2. Create a bootable flash drive with [Rufus][rufus]
3. In system BIOS, temporarily disable Secure Boot
4. Install Windows from flash drive
5. In system BIOS, reenable Secure Boot
6. Enable BitLocker
7. Download networking drivers, transfer via flash drive, and install (if necessary)
8. Run Windows Update for remaining drivers
9. Install any necessary drivers not available via Windows Update
10. Update system BIOS (if necessary)

# Windows configuration
- Review privacy settings
- Review feedback settings
- Review and remove unwanted pre-installed applications
  - [Xbox Game Bar][xbox] and friends
- Review Windows Security settings
  - Automatic sample submission
- Review Windows Update settings
  - [Prevent Windows Update and related wake timers][wake-timers] from waking the computer
- Review power management settings

# Software
- [Chrome]
  - Default browser?
  - Install essential extensions
    - [Ghostery][chrome-ghostery]
    - [uBlock Origin][chrome-ublock]
  - Review settings
    - Disable _Allow Chrome sign-in_
    - Enable _Block third-party cookies_
    - On startup, _Continue where you left off_
- [Visual Studio][vss-vs] Enterprise edition
- [SQL Server][vss-sql] Developer edition
- [Windows Terminal][terminal]
- Office
  1. [Generate a deployment template][odt-config] to exclude apps you don't need (e.g. Access, Skype)
  2. Install with [Office Deployment Tool][odt]

[vss-windows]: https://my.visualstudio.com/Downloads?q=Windows%2010
[vss-vs]: https://my.visualstudio.com/Downloads?q=Visual%20Studio
[vss-sql]: https://my.visualstudio.com/Downloads?q=SQL%20Server
[rufus]: https://github.com/pbatard/rufus
[wake-timers]: https://superuser.com/questions/973009/conclusively-stop-wake-timers-from-waking-windows-10-desktop
[chrome]: https://www.google.com/chrome/
[chrome-ghostery]: https://chrome.google.com/webstore/detail/ghostery-%E2%80%93-privacy-ad-blo/mlomiejdfkolichcflejclcbmpeaniij?hl=en
[chrome-ublock]: https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?hl=en
[terminal]: https://github.com/microsoft/terminal
[xbox]: https://gist.github.com/joshschmelzle/04c57d957c5bb92e85ae9180021b26dc
[odt]: https://www.microsoft.com/en-us/download/details.aspx?id=49117
[odt-config]: https://config.office.com/
