# Windows installation
1. Download a Windows 10 image from [Visual Studio Subscriptions][vss-windows]
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
- Review installed applications
- Review Windows Security settings
  - Automatic sample submission
- Review Windows Update settings
  - [Prevent Windows Update and related wake timers][wake-timers] from waking the computer

[vss-windows]: https://my.visualstudio.com/Downloads?q=Windows%2010
[rufus]: https://github.com/pbatard/rufus
[wake-timers]: https://superuser.com/questions/973009/conclusively-stop-wake-timers-from-waking-windows-10-desktop
