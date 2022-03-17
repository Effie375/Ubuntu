# Install Anaconda

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

The installer prompts "In order to continue the installation process, please review the license agreement." Click Enter to view license terms.

```none
Welcome to Anaconda3 2021.11

In order to continue the installation process, please review the license
agreement.
Please, press ENTER to continue
>>>
```

Scroll to the bottom of the license terms and enter "yes" to agree.

```none
Do you accept the license terms? [yes|no]
[no] >>> yes
```

The installer prompts you to click Enter to accept the default install location, CTRL-C to cancel the installation, or specify an alternate installation directory. If you accept the default install location, the installer displays “PREFIX=/home/<user>/anaconda<2 or 3>” and continues the installation. It may take a few minutes to complete. We recommend you accept the default install location. Do not choose the path as /usr for the Anaconda/Miniconda installation.

```none
Anaconda3 will now be installed into this location:
/home/effie/anaconda3

  - Press ENTER to confirm the location
  - Press CTRL-C to abort the installation
  - Or specify a different location below

[/home/effie/anaconda3] >>>
```

The installer prompts "Do you wish the installer to initialize Anaconda3 by running conda init?" We recommend "yes". If you enter "no", then conda will not modify your shell scripts at all. In order to initialize after the installation process is done, first run `source <path to conda>/bin/activate` and then run `conda init`.

```none
source ~/anaconda3/bin/activate
conda init
```

The installer finishes and displays "Thank you for installing Anaconda<2 or 3>!"

The installer provides a link to install PyCharm for Anaconda at https://www.anaconda.com/pycharm.

Close and open your terminal window for the installation to take effect, or you can enter the command `source ~/.bashrc`.

```none
source ~/.bashrc
```

To control whether or not each shell session has the base environment activated or not, run `conda config --set auto_activate_base False or True`. To run conda from anywhere without having the base environment activated by default, use `conda config --set auto_activate_base False`. This only works if you have run `conda init` first.
