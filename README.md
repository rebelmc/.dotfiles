# Peters Dotfiles

This is my personal  collection of dotfiles and scripts I use for customizing my terminal environment.

The files here are currently used for customizing the following:

- Git
- bin/
- Zsh

The repository should be cloned into your home directory (copy/pasting the installation
commands will do this for you). Dotfiles you wish to keep track of should be located in 
the .dotfiles/dotfiles directory. They will need to have a ".symlink" extention that the 
bootstrap.sh script will use to symlink dotfiles you wish to track in your home directory.

## Installation

The installation is basically cloning all files in a local folder named ".dotfiles" in your home directory and then running the bootstrap script.

```sh
git clone https://github.com/rebelmc/.dotfiles.git ~/.dotfiles
~/.dotfiles/bootstrap.sh
```

## Explanation of Folders

### dotfiles
All your customizations and preferences in one place. Add any "dotfile" you want to take with you
to the dotfiles directory with a '.symlink' extension and it will be automatically added when you
run the bootstrap.sh script. Check out the ones already there for examples.

### bin
Written a script you wish you had saved so you could use it on another system? Add useful scripts 
to the bin directory and they'll be available on any system you clone your dotfiles to. The bin
directory even gets added to your PATH when the bootstrap.sh script is run. No additional setup needed!