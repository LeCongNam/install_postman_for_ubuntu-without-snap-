# install_postman_for_ubuntu-without-snap-
Toturial install Postman on Ubuntu and create shortcut icon

# Goal
[Postman](https://www.postman.com/) is a usefull app to build and test APIs, most commonly installed on ubuntu-like systems via snap. On recent distributions of Linux Mint (20 and above), snap installs are no longer possible. 
The instructions below show how to install Postman via the terminal.
NOTE: why you should be used this toturial? 
- Beacause if you install with snap, cursor is very ```BAD```. It look do not like usual T.T 

### Download Postman
`$ wget https://dl.pstmn.io/download/latest/linux64 -O postman.tar.gz`

### Extract archive
`$ sudo tar -xzf postman.tar.gz -C /opt`

### Make symlink
`$ sudo ln -s /opt/Postman/Postman /usr/bin/postman`

### Optional: Remove downloaded file
`$ rm postman.tar.gz`

### Make Desktop icon
`$ sudo vim /usr/share/applications/postman.desktop`

```
[Desktop Entry]
Encoding=UTF-8
Type=Application
Name=Postman
Icon=/home/lenam/Documents/Postman/app/resources/app/assets/icon.png
Exec="/home/lenam/Documents/Postman/Postman"
Comment=Postman Desktop App
Categories=Application
Terminal=false
```
