# Deploy Windows 10 using Windows Setup

## Checklist

### Requirements

- Get Windows 10 installation media
- Get device drivers
- Get tools
  - [7-zip](https://7-zip.org/)
  - [Internet Download Manager](https://www.internetdownloadmanager.com/)
  - [Shadowsocks for Windows](https://github.com/shadowsocks/shadowsocks-windows)
  - [Windows 8 AppContainer Loopback Utility](https://www.telerik.com/fiddler/add-ons)

### Steps

- Disconnect from the Internet
- Clear the configuration information off the system drive
  - `DISKPART`
  - `SELECT DISK <The DiskPart disk index number of the system drive>`
  - `CLEAN`
- Load the storage driver
- Install Windows on the system drive
- Restart Windows
- Add a second keyboard layout
- Sign in with a local account
- Configure Display
- Configure User Account Control
- Reorder drive letters
- Install device drivers
- Configure Power Options
- Rename the PC
- Restart Windows
- Connect to the Internet
- Configure network profile
- Configure For developers
- Configure Date & Time
  - Configure Time zone
  - Synchronize with an Internet time server
- Sign in with a Microsoft Account
- Activate Windows
- Windows Update
  - Enable `Give me updates for other Microsoft products when I update Windows`
  - Configure Delivery Optimization
  - Check for updates
- Microsoft Store
  - Get updates