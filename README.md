# Sublime Text 3 Configuration

This repository contains a custom configuration for `Sublime Text 3` together with settings and key bindings.
It is used to synchronize the state of the editor among different devices.

## Usage
1. Install `Sublime Text 3` 
2. Open `Sublime Text 3`
3. Open the command palette by typing `ctrl+shift+p`
4. Type `install` and choose the entry `Install Package Control`
5. Close `Sublime Text 3`
6. Open a shell and execute the following commands
```
    cd ~/.config/sublime-text-3/Packages
    rm -rf User/
    git clone https://github.com/lyrahgames/sublime-text-3-config.git User
```
7. Restart `Sublime Text 3` and wait for all packages to be downloaded
8. Close again `Sublime Text 3`
9. Open a shell and execute the following commands
```
    cd ~/.config/sublime-text-3/Packages/User
    git reset --hard HEAD
```
10. Open again `Sublime Text 3` and make sure everything is working

## Spell Checking for Different Languages
To enable spell checking for different languages one first has to install more dictionaries.
Open a shell and run the following commands.
```
    cd ~/.config/sublime-text-3/Packages
    git clone https://github.com/titoBouzout/Dictionaries.git
```
Turn spell checking on and off by pressing `f6` and change the dictionaries by choosing the entry `Dictionaries: Set Language` or `Dictionaries: Set Language (Current View)` in the command palette.

## Customize
Customize the key bindings and the general settings by tweaking the files `Default (Linux).sublime-settings` and `Preferences.sublime-settings`.

## Requirements and Dependencies
- `git`
- `clang`
- `clang-tidy`
- `clang-format`
- `cmake-format`
- `cppcheck`
- TexLive
- `gnuplot`