# Deploy Windows 10 using Windows Setup

## Checklist

### Requirements

- Get Windows 10 installation media
- Get device drivers

### Steps

- Disconnect from the Internet
- Boot to Windows Setup
- Clear the configuration information off the system drive
  - `DISKPART`
  - `SELECT DISK <The DiskPart disk index number of the system drive>`
  - `CLEAN`
- Reboot to Windows Setup
- Select Custom installation
- Load the storage driver
- Install Windows on the system drive
- Add a second keyboard layout
- Sign in with a local account
- Let Cortana respond to "Hey Cortana"
- Configure User Account Control
- Reorder drive letters
- _(Optional)_ Rename system disk
- Install device drivers
- Configure Display
- Configure Sound
- Configure Power Options
- Rename the PC
- Connect to the Internet
- Configure network profile
- Configure Date & Time
  - Configure Time zone
  - Synchronize with an Internet time server
- Configure For developers
- Sign in with a Microsoft account
- Access work or school
- Configure Sign-in options
- Activate Windows
- Configure Windows Insider Program
- Configure Windows Update
  - Configure Active hours
  - Enable `Restart this device as soon as possible when a restart is required to install an update.`
- Configure Delivery Optimization
- Check for updates in Windows Update
- Get updates in Microsoft Store
- Configure OneDrive
  - Configure Auto Save
    - You can't unpin the Desktop folder from Quick access in File Explorer after enabling this feature.
      - [Feedback](https://aka.ms/AA3fe68)
- Configure properties of disk drives and network adapters in Device Manager
- Configure BitLocker
