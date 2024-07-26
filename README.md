# Uninstall-Pyton-Version

## To list all python versions in default locations
ls /usr/bin/python* 
## To remove just python3 package
sudo apt-get remove python3.6

## plus it's dependent packages
sudo apt-get remove --auto-remove python3.6

## plus configuration and/or data files of python3
sudo apt-get purge python3.6

## both configuration and/or data files of python3.5 and it's dependencies
sudo apt-get purge --auto-remove python3.6

## How to install new version of python
sudo apt-get update

sudo apt-get install python3

Also, see https://docs.python-guide.org/starting/install3/linux/
or install python3.8 https://linuxize.com/post/how-to-install-python-3-8-on-ubuntu-18-04/

## ModuleNotFoundError: No module named '_sqlite3'.
- sudo apt-get install libsqlite3-dev
- ./configure --enable-loadable-sqlite-extensions && make && sudo make install

## Last One Think
sudo apt install --reinstall ubuntu-desktop
