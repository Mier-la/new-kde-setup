## Introduction
This repository was made for quickly setting up new KDE-based Linux machines by adding new packages and deleting unnecessary packages pre-installed by KDE. This is done by taking a list of packages in a file and passing them into a package manager. This repository is for my own personal use, but is free to be used by anyone.

## Basic use
### On Arch Distributions
Run the following commands in order:
1. `sudo pacman -Sy $(<add-wanted-packages.list)`
2. `sudo pacman -R $(<remove-kde-packages.list)`
3. `sudo pacman -Qdtq | sudo pacman -Rs -` 
### On Debian/Ubuntu Distributions
Run the following commands in order:
1. `sudo apt install $(<add-wanted-packages.list)`
2. `sudo apt remove $(<remove-kde-packages.list)`
3. `sudo apt autoremove`
