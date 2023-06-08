# Archinstall config files

These config files (`.json`) are used to _"more or less"_ automate the installation of Arch-Linux 
with the help of the [Archinstall](https://archinstall.readthedocs.io/index.html) installscript.

`user_configuration.json`: Contains typical configuration settings like packages, locale, language
keyboardlayout and so on.
`user_disk_layout.json`: Sets the partition layout, filesystemtype & mountpoints.

How it works:
```bash
archinstall --config https://github.com/ckiri/archinstall-config/user_configuration.json \
	    --disk_layout https://github.com/ckiri/archinstall-config/user_disk_layout.json
```
# archinstall-config
