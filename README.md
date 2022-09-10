# What is ripdrag?
ripdrag is an application that lets you drag and drop files from and to the terminal.

It's designed to be feature to feature* compatible with [dragon](https://github.com/mwh/dragon), while being written in modern Rust and GTK4.

*some features like --on-top can't be ported over because of limitations in gtk4
# Use cases

Many applications expect files to be dragged into them. Normally you would have to put your beloved terminal aside and open a file manager to that, but now you can just type ```ripdrag FILENAME``` and be done.

Used in combination with a fuzzy finder like [fzf](https://github.com/junegunn/fzf) - e.g. ```ripdrag $(fzf)``` - can make for an amazingly quick and easy terminal experience. 

# How to install
```
git clone git@github.com:nik012003/ripdrag.git
cd ripdrag
cargo install --path .
```
# Project status
Only a proof of concept has been written for the time being.

Working:
- drag files from the terminal to other applications
- exit after finished dragging
- show icons
- input file paths from stdin

TODO:
- drag files from other apps to the terminal
- clean up code
- pacman, deb, rpm, windows and macos build scripts
- automated builds