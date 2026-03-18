# my-configs

clean, minimal hyprland dotfiles built around a coding stack on arch linux. open source and free to use.

---

## screenshots

> coming soon

---

## what's included

| config | description |
|--------|-------------|
| hyprland | window manager config with custom keybinds |
| alacritty | terminal with tokyo night colors and 0.6 opacity |
| starship | minimal prompt with git, python and time |

---

## dependencies

| package | purpose |
|---------|---------|
| hyprland | window manager |
| waybar | status bar |
| alacritty | terminal |
| wofi | app launcher |
| hyprpaper | wallpaper |
| hyprlock | screen lock |
| hypridle | idle daemon |
| dunst | notifications |
| librewolf | browser |
| vesktop | discord client |
| wl-clipboard | clipboard support |
| hyprshot | screenshots |
| brightnessctl | brightness control |
| pamixer | audio control |
| starship | shell prompt |
| ttf-jetbrains-mono-nerd | nerd font |
| papirus-icon-theme | icon theme |

---

## installation

> requires arch linux with hyprland and stow installed

```bash
# install stow, starship, git and base-devel
sudo pacman -S stow starship git base-devel

# clone the repo
git clone https://github.com/noah-or13/my-configs.git ~/dotfiles

# symlink configs
cd ~/dotfiles && stow .

# add starship to your shell
echo 'eval "$(starship init bash)"' >> ~/.bashrc
source ~/.bashrc
```
```
# install yay with git
git clone https://aur.archlinux.org/yay-bin.git
cd ~/yay-bin
makepkg -si
# then install AUR packages
yay -S hyprshot librewolf-bin vesktop-bin waypaper
```
---

## keybinds

### apps

| keybind | action |
|---------|--------|
| `SUPER + Q` | open terminal |
| `SUPER + B` | open browser |
| `SUPER + D` | open discord |
| `SUPER + E` | open file manager |
| `SUPER + SPACE` | open app launcher |

### windows

| keybind | action |
|---------|--------|
| `SUPER + C` | close window |
| `SUPER + V` | toggle floating |
| `SUPER + F` | fullscreen |
| `SUPER + P` | pseudotile |
| `SUPER + arrows` | move focus |

### workspaces

| keybind | action |
|---------|--------|
| `SUPER + 1-10` | switch workspace |
| `SUPER + SHIFT + 1-10` | move window to workspace |
| `SUPER + S` | toggle scratchpad |
| `SUPER + SHIFT + S` | send to scratchpad |
| `SUPER + scroll` | cycle workspaces |

### mouse

| keybind | action |
|---------|--------|
| `SUPER + left click drag` | move window |
| `SUPER + right click drag` | resize window |


### media

| keybind | action |
|---------|--------|
| `XF86AudioRaiseVolume` | volume up |
| `XF86AudioLowerVolume` | volume down |
| `XF86AudioMute` | mute |
| `XF86AudioMicMute` | mute mic |
| `XF86MonBrightnessUp` | brightness up |
| `XF86MonBrightnessDown` | brightness down |
| `XF86AudioPlay` | play/pause |
| `XF86AudioNext` | next track |
| `XF86AudioPrev` | previous track |

---

## license

Copyright (c) 2026 noah-or13 — free to use and modify for personal use, credit required, no commercial use permitted.

---

<p align="center">made by <a href="https://github.com/noah-or13">noah-or13</a></p>
