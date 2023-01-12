# macOS-Install

⚠️ This scripts is not done. Use at your own responsibility! ⚠️

----

Install helper for macOS than runs in the Mac Recovery mode.

`install` will ask you if you want to delete your drive and acts accordingly.

You will be able to choose the macOS Version you want, it downloads that one, sets everything up and runs it.

Start the setup by running the following in line in the Terminal in Recovery Mode:

```bash
bash < <(curl -s raw.githubusercontent.com/konfigurate/mosinstall/main/install)
```

On Intel, it does not seem to allow downgrades from the Ventura Recovery, might work on M1.

|Recovery Mode Version|Big Sur|Monterey|Ventura
|:--|:-:|:-:|:-:|
|Catalina|✅|✅|✅|
|Big Sur|✅|✅|✅|
|Monterey|✅|✅|✅|
|Ventura|❌|❌|✅|