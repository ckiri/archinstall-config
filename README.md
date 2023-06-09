# Archinstall config files

These config files (`.json`) are used to _"more or less"_ automate the installation of Arch-Linux 
with the help of the [Archinstall](https://archinstall.readthedocs.io/index.html) installscript.

**Files**:
- `user_configuration.json`: Contains typical configuration settings like packages, locale, language
keyboardlayout and so on.
- `user_disk_layout.json`: Sets the partition layout, filesystemtype & mountpoints.

How it works:
```bash
archinstall --config https://raw.githubusercontent.com/ckiri/archinstall-config/main/user_configuration.json \
	    --disk_layout https://raw.githubusercontent.com/ckiri/archinstall-config/main/user_disk_layout.json
```

Or if you prefer the files locally:
```bash
git clone https://github.com/ckiri/archinstall-config
cd archinstall-config
archinstall --config user_configuration.json --disk_layout user_disk_layout.json
```
