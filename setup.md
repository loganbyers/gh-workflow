Steps/preparation:
 
Install Python3:
Download the "MacOS 64-bit Installer": https://www.python.org/downloads/release/python-374/
Install the .pkg
verify it is installed by opening the terminal and typing `python3 --version`
 
Install pip:

Download the pip installer "get-pip.py" and save in your Home directory: https://bootstrap.pypa.io/

Install pip using the terminal: run `python3 get-pip.py --user `

Verify pip is installed: run `pip --version` (ensure the output mentions python 3.7, not python 2.x)

 

 

Install git:

First, verify git is not yet installed: `run git --version` if a version is printed you are fine, otherwise....

Download the git installer - scroll down to the FAQs to see which version you need: https://sourceforge.net/projects/git-osx-installer/files/

Install like a normal Mac application

Verify it is installed: `run git --version`

 

Install git-lfs:

Follow these instructions for Mac. Disregard the 'Homebrew/Macports' comments: https://help.github.com/en/articles/installing-git-large-file-storage

 

Install pyinvoke:

In the terminal, run `pip install invoke --user`

#activate/deactivate virtual enviornment
Invoke looks for tasks.py file, within which venv is defined, creates venv folder locally
```
virtualenv?
python3 -m venv
echo $PATH
ls -a
open -a TextEdit .bash_profile
*add in file export PATH="$HOME/.local/bin:$PATH"
```
```
pwd
mkdir MY_DIRECTORY_NAME?
cd 
git clone https://github.com/wri/gcom-ghg-inventory
cd gcom-ghg-inventory

virtualenv?
invoke venv
. activate_venv
invoke test
ls venv/bin
echo $PATH
invoke server
deactivate
```
