# macOS-Install

⚠️ This scripts is not done. Use at your own responsibility! ⚠️

----

`mosinstall` was made to force a specific version of macOS in the Recovery Mode of Macs. By downloading the installer directly, we can download the version required and run the program from within the Recovery Mode.

`install` will ask you if you want to delete your drive and acts accordingly. On Catalina, I saw on several occasions, that it might have problems deleting the drive. You'll have to delete the drive yourself.

You will be able to choose the macOS Version you want, it downloads that one, sets everything up and runs it on the spot.

Start the setup by running the following in line in the Terminal in Recovery Mode:

```bash
curl -s raw.githubusercontent.com/konfigurate/mosinstall/main/install | bash
```

## Version Compatibility

- Mojave and older

    When using Mojave, I had problems getting curl to work. Also when downlaoded, the Installer would always ask for an administrator password, which is not set in the recovery. Using the Mojave Recovery will therefore not work.

- Catalina, Big Sur and Monterey

    Using the Recovery for those three Versions supports the installation of all three Versions:

    - Big Sur
    - Monterey
    - Ventura

- Ventura

    The Ventura Recovery doesn't support downgrading to other Versions of macOS, so you can only install Ventura from here.

    You may have success using Shift+Option+Command+R to boot in an older Recovery, but Mojave or older won't work, as already described.