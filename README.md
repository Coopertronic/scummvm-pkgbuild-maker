# scummvm-pkgbuild-maker
This is a QT desktop application that helps you to easily make a `PKGBUILD` for scummvm games.

## Overview

The app is intended so that anyone can create a `PKGBUILD` for any scummvm game and install it with a desktop icon. This icon will launch the game without the user having to go through the scummvm app to start it, just double click the icon on the desktop.

The app will ask for the following things:

- The location of the game folder.
- The game icon.
- The name of the game (it will suggest a package name. The user will be able to change this.

The app will create all the things that are needed and save everything to a zip file.

### Using the `PKGBUILD`

The app will have created the following things in the zip file:

- The `PKGBUILD` file.
- The install script used by the `PKGBUILD` file called `<game-name.install.sh>`.
- A folder called `assets` where all the assets are stored.
- A script that will pull all the assets out of the folder for you, run `makepkg -i` to install it for you and then cleans up the folder. 

### Future ideas

Once the `PKGBUILD` has been made then it would be a nice touch if the app offered to install it for you. 

A batch mode to make and/or install multiple `PKGBUILD` scummvm games 
