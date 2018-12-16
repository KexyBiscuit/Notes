# Deploy Windows 10 using Windows Setup

## Checklist

### Requirements

- Get Windows 10 installation media
- Get device drivers
- _(Optional)_ Get tools
  - [7-zip](https://7-zip.org/)
  - [Internet Download Manager](https://www.internetdownloadmanager.com/)
  - [Shadowsocks for Windows](https://github.com/shadowsocks/shadowsocks-windows)
  - [Visual Studio Code](https://code.visualstudio.com/)
  - [Windows 8 AppContainer Loopback Utility](https://www.telerik.com/fiddler/add-ons)

### Steps

- Disconnect from the Internet
- Boot to Windows Setup
- Clear the configuration information off the system drive
  - `DISKPART`
  - `SELECT DISK <The DiskPart disk index number of the system drive>`
  - `CLEAN`
- Select Custom installation
- Load the storage driver
- Install Windows on the system drive
- Add a second keyboard layout
- Sign in with a local account
- Configure User Account Control
- Reorder drive letters
- _(Optional)_ Rename system disk
- Install device drivers
- Configure Display
- Configure Power Options
- Rename the PC
- Connect to the Internet
- Configure network profile
- Configure Date & Time
  - Configure Time zone
  - Synchronize with an Internet time server
- Configure For developers except for Use developer features
- Sign in with a Microsoft Account
- Configure Sign-in options
- Activate Windows
- Configure Windows Insider Program
- Configure Windows Update
  - Configure Active hours
  - Enable `Give me updates for other Microsoft products when I update Windows`
- Configure Delivery Optimization
- Check for updates in Windows Update
- Configure Use developer features
- Get updates in Microsoft Store
- Configure OneDrive
  - Enable Files On-Demand
  - Configure Auto Save
    - You can't unpin the Desktop folder from Quick access in File Explorer after enabling this feature.
      - [Feedback](https://aka.ms/AA3fe68)
- Configure BitLocker
- Configure Feedback Hub
- Configure To-Do
- Configure Mail
