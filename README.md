# fetchstuck

A Homestuck-themed system fetch tool written in Bash. It re-contextualizes standard Linux system information (OS, Kernel, Uptime, etc.) into Homestuck terminology (Session, Timeline, Session Age).

# Features

Thematic Mapping: Automatically determines your "Class" (based on your Shell) and "Aspect" (based on your Distro).

Custom ASCII: Includes custom condensed "Sburb" house ASCII art.

Image Support: Supports displaying images using kitty (icat) or chafa fallback.

Lightweight: Written in pure Bash with minimal dependencies.

# Installation

Download the script:

git clone [git@github.com:GrandDiJay/fetchstuck.git ](https://github.com/GrandDiJay/fetchstuck.git)
cd fetchstuck



# Make the script executable:

chmod +x fetchstuck



(Optional) Move it to your path to run it from anywhere:

sudo mv fetchstuck /usr/local/bin/



# Usage

Simply run the script:

./fetchstuck



# Options

-h, --help: Show help message.

-v, --version: Show version information.

# Configuration

The script looks for a config file at ~/.config/fetchstuck/config. If it doesn't exist, default values are used.

# Example Configuration:
```
FS_ASCII_ART="sburb"
FS_COLOR_THEME="default"   # Options: default, scratch, grimdark
FS_CUSTOM_TITLE=""         # Set a custom title string
FS_SHOW_GPU="on"           # Toggle GPU detection
FS_IMAGE="/path/to/img.png" # Path to an image to use instead of ASCII
```

# Dependencies

bash

coreutils (awk, sed, grep, cut)

tput (ncurses) - For colors and cursor positioning.

Optional:

lspci (pciutils) - For GPU detection.

chafa - For image display in other terminals.

# License

MIT
