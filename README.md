# Dotfiles and Configurations

## ~/.dotfiles

### Installation
* clone repo to home directory
* create symbolic links

```Shell
cd ~
git clone https://github.com/camjm/.dotfiles.git ~/.dotfiles
ln -s ~/.dotfiles/Git/.gitconfig ~/.gitconfig
ln -s ~/.dotfiles/Git/.gitignore ~/.gitignore_global
ln -s ~/.dotfiles/Git/.stCommitMsg ~/.stCommitMsg
ln -s ~/.dotfiles/Shell/.zprofile ~/.zprofile
ln -s ~/.dotfiles/Shell/.zshrc ~/.zshrc
```

### Note
Use the Homebrew package manager to install software such as VS Code, so you can automatically reinstall from the brewfile to bootstrap a new machine.

`brew bundle dump --describe`

This creates a file that shows the software that has been installed via Homebrew (it keeps track of what it has installed).
You can then copy this file to another machine and run it to install the sloftware.

`brew bundle --file ~/.dotfiles/Brewfile`