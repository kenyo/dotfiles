# dotfiles
Personal configuration files for day-to-day tools

On new device, copy the below snippet in home directory:

``` bash

# setup config
echo "alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'" >> .profile
echo ".cfg" >> .gitignore
git clone --bare git@github.com:kenyo/dotfiles.git $HOME/.cfg


git config --global core.excludesfile ~/.gitignore_global
config config --local status.showUntrackedFiles no


pip install powerline-status

```
