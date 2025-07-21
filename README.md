# Dotfiles Repository

These dotfiles are organized for easy management and deployment using chezmoi. Each tool's configuration is stored in its respective directory, allowing modular updates and portability across systems.

## Table of Contents

- [Waybar](#waybar)
- [Tmux](#tmux)
- [Hyprland](#hyprland)


## Waybar

Waybar is a customizable status bar for Wayland compositors.  
This repository provides a custom CSS stylesheet for Waybar, located at `private_dot_config/waybar/style.css`.

**Features:**
- FontAwesome and system font support
- Semi-transparent backgrounds and custom colors
- Rounded workspace buttons with focused/urgent/hover states
- Module-specific styles (clock, battery, CPU, memory, disk, network, audio, tray, etc.)
- Battery alerts with blinking animation for critical state
- Power profile colors (performance, balanced, power-saver)
- Audio/media module styles
- Privacy indicators for screenshare, audio-in, audio-out
- Scratchpad and keyboard lock indicators
- Responsive margins and padding

**Usage:**
1. Install Waybar ([instructions](https://github.com/Alexays/Waybar))
2. Install FontAwesome:
   ```sh
   sudo pacman -S otf-font-awesome   # Arch Linux
   sudo apt install fonts-font-awesome # Debian/Ubuntu
   ```
3. Copy `style.css` to your Waybar config:
   ```sh
   mkdir -p ~/.config/waybar
   cp style.css ~/.config/waybar/style.css
   ```
4. Reference it in your Waybar config:
   ```json
   "style": "~/.config/waybar/style.css"
   ```

## Tmux

Tmux configuration files (if present) are managed in this repository. They allow for custom keybindings, themes, and workflow optimizations for terminal multiplexing.  
*(Add details here if you have a `.tmux.conf` or related files.)*

## Hyprland

Hyprland configuration files (if present) are managed here to customize your Wayland compositor experience, including window management, keybindings, and appearance.  
*(Add details here if you have a Hyprland config.)*

