# Update Bitwarden Script

This script, update-bitwarden.sh, automates the process of updating rpm installs of Bitwarden on your system.

Adapted from a script provided by aloksharma [here](https://community.bitwarden.com/t/guide-automating-bitwarden-updates-on-linux-deb-package/82232).

## Usage

To use this script, simply run it from the command line:

```shell
./update-bitwarden.sh
```

The script will attempt the latest rpm installation if not currently installed or if the current installation is not the latest.

## Requirements

- Must be an OS supported by the rpm distribution of Bitwarden. See [here](https://bitwarden.com/download/).
- Must be run with the necessary permissions to install/update Bitwarden
- Must have dnf installed

## Scheduling

You can schedule this task to run via cron daily with the following:

```shell
sudo ln -s /path/to/update_bitwarden.sh /etc/cron.daily/
```
