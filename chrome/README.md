# Install Google Chrome Browser on Ubuntu 20.04

If you installed the minimal Ubuntu 20.04, chances are, you do not have Chrome browser installed. Therefore, follow this guide to learn how to install Google Chrome Browser on Ubuntu 20.04.

You can install Google Chrome browser by downloading the Debian binary package or by simply installing the Chrome sources lists and then installing the Chrome browser from these sources lists.

## Update System Package Cache

Before you can proceed, update your package cache.

```none
sudo apt update
```

## Install Google Chrome using DEB Binary Package

Download Google Chrome DEB binary package from Google Chrome page.

```none
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb -P /tmp
```

Then install it using APT so as to deal with required dependencies automatically.

```none
sudo apt install /tmp/google-chrome-stable_current_amd64.deb
```

The latest Google Chrome browser has been installed on Ubuntu 20.04;

```none
google-chrome --version
```

## Running Google Chrome Browser on Ubuntu 20.04

You can now launch Google Chrome browser from activities on Ubuntu 20.04.

You can as well launch Google chrome browser from your terminal by running either of the commands below;

```none
google-chrome
```

That is how easy the installation of Google Chrome Browser on Ubuntu 20.04 is.

## Uninstall Chrome in Ubuntu 20.04

```none
sudo apt-get remove google-chrome-stable
```
