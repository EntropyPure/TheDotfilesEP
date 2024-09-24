# EntropyPure's Dotfiles-EP

My personal Dotfiles-Repo for my Arch Hyprland environment.

Includes Hyprland dots as well as my application dots.

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


```
sudo pacman -S hyprland kitty nvim dunst polkit-kde-agent xdg-desktop-portal-hyprland waybar wpaperd swaylock swayidle hyprshot wofi 
```

### Chezmoi Setup

Install using pacman:

```
pacman -S chezmoi
```


