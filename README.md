Dotfiles combining Hyprland config, Quickshell config, and all other interconnected programs, required to run full DE.

Install instructions:
Cloning repo directly into ~/.config will not be possible, as git does not allow cloning into non-empty directories.
The easiest way would be to clone into /tmp and copy content to .config:
'''
git clone git@github.com:QuantumKoga/dotfiles.git /tmp/dotfiles

cp -a /tmp/dotfiles/. ~/.config/

rm -rf /tmp/dotfiles
'''
