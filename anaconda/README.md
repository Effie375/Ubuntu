# Install Anaconda on Ubuntu 20.04

Anaconda is a package manager used in scientific computing and data science. It’s designed to provide scientific libraries and dependencies in the Python programming language. Anaconda is commonly used for machine learning and artificial intelligence applications.

This step by step guide will show you how to install Anaconda on an Ubuntu 20.04 system.

## Prerequisites

- A user account with `sudo` privileges
- Access to a command line/terminal window (Ctrl-Alt-T)

## Update Local Package Manager

Start by updating the local package manager. Open a terminal window and enter the following:

```none
sudo apt-get update
```

## Download the Latest Version of Anaconda

Switch to the /Downloads directory and download the [Anaconda installer](https://www.anaconda.com/products/individual#linux) for Linux:

```none
cd /Downloads
```

## Run Anaconda Installation Script

The Anaconda installer is a **bash script**. To run the installation script, use the command:

```none
bash Anaconda3-2021.11-Linux-x86_64.sh
```

A license agreement will appear. Use the **Enter** key to review the agreement.

```none
Welcome to Anaconda3 2021.11

In order to continue the installation process, please review the license
agreement.
Please, press ENTER to continue
>>>
```

At the bottom, type **yes** to agree to the terms.

```none
Do you accept the license terms? [yes|no]
[no] >>> yes
```

The installer will prompt you to accept the default location, or install to a different location. Use the default path unless you have a specific need to change it. (You may cancel the installation here if needed.)

```none
Anaconda3 will now be installed into this location:
/home/effie/anaconda3

  - Press ENTER to confirm the location
  - Press CTRL-C to abort the installation
  - Or specify a different location below

[/home/effie/anaconda3] >>>
```
