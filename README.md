# EntropyPure's Dotfiles-EP

My personal Dotfiles-Repo for my Arch Hyprland environment.

Includes Hyprland dots as well as my application dots.

## Setup

These are my personal notes to help myself should I ever bork up my Arch so hard, I have to reinstall. Packages, setup steps etc.

### Required packages

#### AUR Helper

Would love to use paru because RUST, but setup failed last time (Please try again, future me!).

So we go for the next best thing: yay

```
sudo pacman -S --needed git base-devel
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```

### Chezmoi Setup

Install using pacman or yay:

```
yay -S chezmoi
```

