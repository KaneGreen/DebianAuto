# Debian 11 Semi-automatic Installation Preseed

## Documentation
[Debian official documentation for Preseed](https://wiki.debian.org/DebianInstaller/Preseed)

## Content
* This Preseed file does not contain network configuration and disk partitions,
so these two need to be manually configured by the user.
* The `apt` mirror is set to `http://mirrors.ustc.edu.cn/debian`, with `non-free` and `contrib` enabled, but `deb-src` disabled, and  the Popularity Contest are opt-in.
* The system language is `en_US.UTF-8`, the time zone is `Hong Kong` (UTC+8), and time synchronization is enabled.
* The username is `user`, the password is `123456`, and `sudo` has been set. Disable the root account.
* Desktop environment is not installed.
* `Standard System Utilities` and `SSH Server` are installed.
* `curl` and `htop` are installed.
* After the installation is complete, it will automatically restart without prompting.
* Currently only tested on Debian 11 installation DVD images.

## Usage
Please load this file `preseed.cfg` for Debian installer.
