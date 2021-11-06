## Introduction
This repository was made for quickly setting up new KDE-based Linux machines by adding new packages and deleting unnecessary packages pre-installed by KDE. This is done by taking a list of packages in a file and passing them into a package manager. This repository is for my own personal use, but is free to be used by anyone.

## Basic use
### On Arch Distributions
Run the following commands in order:
1. `sudo pacman -Sy $(<add-wanted-packages.list)` - Add packages contained within add-wanted-packages.list.
2. `sudo pacman -R $(<arch-remove-kde-packages.list)` - Remove packages contained within remove-kde-packages.list.
3. `sudo pacman -Qdtq | sudo pacman -Rs -` - Remove any packages no longer used. If there is an  error claiming there is an empty stdin, it means there are no unused packages on the system.
### On Debian/Ubuntu Distributions
Run the following commands in order:
1. `sudo apt install $(<add-wanted-packages.list)` - Add packages contained within add-wanted-packages.list.
2. `sudo apt remove $(<debian-remove-kde-packages.list)` - Remove packages contained within remove-kde-packages.list
3. `sudo apt autoremove` - Remove any packages no longer used.
