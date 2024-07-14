# Pacman Aliases

Pacman Aliases is a comprehensive collection of Bash aliases and automatic installation scripts tailored to streamline package management on Arch Linux systems using `pacman`. These aliases provide intuitive shortcuts for common package operations, enhancing efficiency and ease of use in your daily system administration tasks.

## Features

**Aliases for Pacman Commands**: Simplified and memorable commands that mirror original `pacman` operations:
- `install` (`i`, `add`): Install a package (`pacman -S`).
- `update`: Update package database (`pacman -Sy`).,
- `upgrade`: Upgrade all packages (`pacman -Syu`).
- `search`: Search for a package (`pacman -Ss`).
- `info`: Display detailed information about a package (`pacman -Si`).
- `autoremove`: Remove orphaned dependencies (`pacman -Qdtq | pacman -Rs -`).
- `remove` (`uninstall`, `delete`): Remove a package (`pacman -R`).
- `purge` (`fullremove`, `fulluninstall`): Remove a package along with its configuration files (`pacman -Rns`).
- `clean` (`autoclean`): Clean package cache (`pacman -Sc`).
- `mirrors` (`mirrorlist`): List and manage mirrors (`pacman-mirrors -g`).
- `listpackages` (`lsp`): List installed packages (`pacman -Q`).
- `list` (`ls`, `listrepos`, `lsr`): List packages along with their repositories (`pacman -Sl`).
- `config` (`editrepos`): Display or edit Pacman configuration file (`nano /etc/pacman.conf`).
- `addmirror`: Add a specified mirror to the mirrorlist file.
- `reinstall`: Reinstall a package (`pacman -S --overwrite '*'`).
- `version` (`v`): Display Pacman version information (`pacman --version`).
- `help` (`-h`, `h`): Display Pacman help page (`pacman --help`).
- `aliases` (`alias`, `aliaseshelp`): Display Pacman Aliases help page.
- `autoinstall`: Displays Pacman Aliases automatic installation scripts. (⚠️READ BELOW)

Of course! You can still use pacman commands like `pacman -S`.

**Automatic Installation Scripts**: Includes scripts for installing additional software like:
- `yay`: Installs Yay AUR helper on your system.
- `kdediscover`: Adds Pacman and Flatpak packages to KDE software manager. (Enables multilib repository if not enabled.)
- `wine`: Enables running Windows applications on your system. DXVK is installed for games. (Enables multilib repository if not enabled.)
- `bluetooth`: Installs bluez packages for Bluetooth via AUR (yay).
- `nvidia`: Installs NVIDIA drivers and optimus drivers if available for your laptop. (NOT RECOMMENDED, READ WARNING)

⚠️ **_IMPORTANT WARNING: These automatic installation scripts are not thoroughly tested and are not actively maintained. We recommend manual installation of packages instead._**

**Multilingual Support**: Displays messages in English and Turkish based on system language settings. If you want to add your own language to here, you can contribute to the project.

## Usage

### Installing Pacman Aliases

1. Clone the repository and compile:
```bash
git clone https://github.com/cfy8001/pacman-aliases.git
cd pacman-aliases
makepkg -si
```

### Using Pacman Aliases

Once installed, use the `pacman` command followed by one of the aliases listed above to perform the corresponding package management operation.

### Contributing

Contributions are welcome! If you find a bug, have suggestions for improvements, or want to add more aliases, please create an issue or submit a pull request.

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

### Disclaimer

**Use at Your Own Risk**: These automatic installation scripts are not actively maintained, not thoroughly tested, provided as-is and may not cover all edge cases. It's recommended to review and adapt scripts according to your system's specific requirements. Always exercise caution when making system-level changes.
