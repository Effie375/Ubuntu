# Installing pip for Python 3

Ubuntu 20.04 ships with Python 3, as the default Python installation. Complete the following steps to install `pip` (pip3) for Python 3:

```none
sudo apt update
```

Use the following command to install pip for Python 3:

```none
sudo apt install python3-pip
```

The command above will also install all the dependencies required for building Python modules.

Once the installation is complete, verify the installation by checking the pip version:

```none
pip3 --version
```

The version number may vary, but it will look something like this:

```none
pip 20.0.2 from /usr/lib/python3/dist-packages/pip (python 3.8)
```
