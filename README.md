![alt text](https://github.com/Annamorphismus/alacritty_config/blob/main/alacritty_terminal.png)
# alacritty_config
Alacrity Terminal config paired with Zsh configuration with Antigen and Oh-My-Zsh


## Installation of Alacritty on OpenSuse Tumbleweed

1.Install extra libraries

    zypper install cmake freetype-devel fontconfig-devel libxcb-devel libxkbcommon-devel


2. Clone Source Code

        git clone https://github.com/alacritty/alacritty.git
        cd alacritty

5. Install Rust Compiler

        rustup.rs .

6. Build Release

        cargo build --release

8. Make Desktop Entry

        sudo cp target/release/alacritty /usr/local/bin # or anywhere else in $PATH
        sudo cp extra/logo/alacritty-term.svg /usr/share/pixmaps/Alacritty.svg
        sudo desktop-file-install extra/linux/Alacritty.desktop
        sudo update-desktop-database

## Config Alacritty
  Use the given alacritty.toml file to configurate the Alacritty Terminal.
  
  Path:
  
    ~/.config/alacritty/alacritty.toml


# ZSH Config 

## Install ZSH 

    sudo zypper in zsh 

## Make ZSH default

    chsh -s /bin/zsh

## Install Antigen

    curl -L git.io/antigen > antigen.zsh

## Configure ZSH 

You can configure your Oh-My-Zsh directly in your .antigenrc file. A example file is given.

Path:

      ~/.antigenrc


# Theme powerlevel10k
If you want to use the powerlevel10k Theme you have to follow the instruktions form https://github.com/romkatv/powerlevel10k

# Tmux
For better handling of the console you can consider using tmux 

