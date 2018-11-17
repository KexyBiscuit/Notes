# Error occurs while using Git for Windows with user.signingkey config setting

## Symptoms

If you set the `user.signingkey` config setting in Git for Windows, and you were not using the `gpg` program bundled with it (that means, you installed and configured GnuPG yourself), git commands that require GnuPG may generates the following error message:

```powershell
gpg: directory '/c/Users/<User>/.gnupg' created
gpg: keybox '/c/Users/<User>/.gnupg/pubring.kbx' created
gpg: skipped "<YOUR SINGINGKEY>": No secret key
gpg: signing failed: No secret key
error: gpg failed to sign the data
fatal: failed to write commit object
```

## Cause

Git for Windows comes with MSYS2, providing a number of packages, including GnuPG. Because of this, Git for Windows would use its own `gpg` as default, even if you have one in PATH. However, GnuPG from Git for Windows could be obsolute, or even worse, it could use different configuration files from yours. This causes many problems, and one of them is shown above.

## Resolution

To resolve this problem, follow these steps:

1. Configure Git for Windows to use your own GnuPG installation. You can run the following command in Windows Powershell:

    ```powershell
    git config --global gpg.program (Get-Command gpg.exe).Path
    ```
2. Restart every program using Git for Windows.
