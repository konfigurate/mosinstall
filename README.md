# macOS-Install aka. mosinstall

`mosinstall` was made to force the download of a specific version of macOS in the macOS recovery mode.

`install` will ask you if you want to delete your drive and acts accordingly. On Catalina, I saw on several occasions, that it might have problems deleting the drive. You'll have to delete the drive yourself.

You will be able to choose the macOS Version you want, it downloads that one, sets everything up and runs it on the spot.

Start the setup by running the following in line in the Terminal in Recovery Mode:

```bash
curl -s raw.githubusercontent.com/konfigurate/mosinstall/main/install | bash
```

## Recovery Version Compatibility

- Mojave and older won't work

    When using Mojave, I had problems getting curl to work. Also when downlaoded, the Installer would always ask for an administrator password, which is not set in the recovery. Using the Mojave Recovery will therefore not work.

- Catalina, Big Sur and Monterey

    Using the Recovery of those three Versions supports the installation of all three Versions:

    - Big Sur
    - Monterey
    - Ventura

- Ventura

    The Ventura Recovery doesn't support downgrading to other Versions of macOS, so you can only install Ventura from here.

    You may have success using Shift+Option+Command+R to boot in an older Recovery, but Mojave or older won't work, as already described.