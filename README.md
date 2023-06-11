# KingOfTheHomer
Easily configurable King of the Hill themed [Homer dashboard](https://github.com/bastienwirtz/homer).

## Configuration & Usability
I couldn't quite determine what style I wanted for this template, so I made sure the `config.yml` file is fairly commented and verbose to provide easy modification.
If you use the `install.sh` script, a symbolic link is created in the current user's root directory for easier editing.

#### Standard Light Theme
![Light w/o Searchbar](https://cdn.discordapp.com/attachments/855920119292362802/1117548075452481566/image.png)

#### Cursed Dark Theme with a DuckDuckGo Searchbar
![Dark w/ Searchbar](https://cdn.discordapp.com/attachments/855920119292362802/1117548417976127644/image.png)

## Installation
The `install.sh` script is based off of my [ProxmoxMaster](https://github.com/tylerdotrar/ProxmoxMaster) repository.
This script automatically installs `Homer` and `KingOfTheHomer` from scratch, while providing user input and automation for port selection and SSL utilization.

One-liner to install both `Homer` and `KingOfTheHomer` (tested on an Ubuntu 22.04 LXC):
```shell
bash -c "$(wget -qO- https://github.com/tylerdotrar/KingOfTheHomer/raw/main/install.sh)"
```
![install.sh](https://cdn.discordapp.com/attachments/855920119292362802/1117573926319554620/image.png)

Manual installation into an existing `Homer` instance:
```shell
git clone https://github.com/tylerdotrar/KingOfTheHomer
cp -rf KingOfTheHomer/assets /var/www/homer
rm -rf KingOfTheHomer
```

## Credits
- Credit to [bastienwirtz](https://github.com/bastienwirtz) for the original [Homer](https://github.com/bastienwirtz/homer) project.
- Credit to [walkxcode](https://github.com/walkxcode) for his custom [Homer theme](https://github.com/walkxcode/homer-theme) for giving me a great baseline.
