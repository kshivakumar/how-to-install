## Ubuntu 16.04(xenial)

The below steps will not alter/remove the incumbent Python version OS uses. Also, multiple versions of Python can be installed and maintained using these steps.

1. `sudo apt-get install build-essential checkinstall`
2. `sudo apt-get install libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev libffi-dev liblzma-dev`
3. `cd /usr/src` or any temp directory.  
_Replace `3.7.3` with the required version in the below steps._
4. `sudo wget https://www.python.org/ftp/python/3.7.3/Python-3.7.3.tgz`.
5. `sudo tar xzf Python-3.7.3.tgz`; `cd Python-3.7.3`
6. `sudo ./configure --enable-optimizations`
7. `sudo make altinstall` -  _make altinstall_ will ensure the existing Python version(s) are not affected.

Reference:
https://tecadmin.net/install-python-3-7-on-ubuntu-linuxmint/

#### Creating a virtualenv
`python3.7 -m venv /path/to/new/venv`
