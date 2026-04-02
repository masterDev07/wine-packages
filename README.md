Installation:

```bash
sudo dpkg -i wine1002_1.0_all.deb
```

To run this custom Wine same as release version:

Example
Wine version 10.2

```bash
wine1002 --version
```

Add to .bashrc to run application on bin directory
```bash
export PATH="$PATH:/opt/wine1002/bin"
```

### Explanation

- Wine is installed in `/opt/wine1002` to avoid conflicts with other Wine packages.
- The postinst script creates a symlink in `/usr/local/bin` for easy access.
- This package runs in parallel with other Wine packages and does not replace the default Wine version on your system.
- You can choose which Wine version to use by calling `wine1002` or the regular `wine`.
