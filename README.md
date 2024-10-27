# EntropyPure's The Dotfiles-EP

Personal Dotfiles-Repo for my Arch Hyprland environment.

Includes dotFiles for Hyprland as well as my applications.

## Setup

These are my personal notes to help myself should I ever bork up my Arch so hard, I have to reinstall. Packages, setup steps etc.

### Good Manners

Create a git_clones directory:

```
mkdir ~/git_clones
```

To keep it all in one place!

### Required packages

#### AUR Helper

##### paru

If it builds, you should use it, because RUST.

```
sudo pacman -S --needed base-devel
cd ~/git_clones
git clone https://aur.archlinux.org/paru.git
cd paru
makepkg -si
```

##### yay

If it does not build, we go for the next best thing: yay

```
sudo pacman -S --needed git base-devel
cd ~/git_clones
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```

#### Install these first

Install these packages first, after applying the config with chezmoi everything should be more or less set.

```
sudo pacman -S hyprland hyprlock hypridle hyprshot fastfetch kitty chezmoi nvim yazi wlogout sddm swaync starship polkit-kde-agent xdg-desktop-portal-hyprland waybar wpaperd wofi firefox
```


### Chezmoi Setup

First things first: install SSH-Key for GitHub access.

Install the package using pacman, if not already installed:

```
pacman -S chezmoi
```

#### Apply dotFiles from git repo

```
chezmoi init --apply https://github.com/EntropyPure/TheDotfilesEP.git
```

If all went as it should, the setup is done and Hyprland including apps up and running.
