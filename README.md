# Bwhite.dev's Toolset

I made this project to make setting up my computers a little easier. It has a terminal menu for installing apps, developer tools, and some of my personal configs.

## What it does

- **macOS:** Installs apps and dev tools with Homebrew, sets up Zsh and Starship, and installs my Neovim config.
- **Windows:** Runs PowerShell scripts for apps and dev tools using Chocolatey, with options for Windows activation and shell setup.
- **Linux:** Installs my Neovim config or adds settings from the included `zshrc` to `.bashrc`. This part is still pretty basic.

The script detects your OS and shows the menu for it. It also checks for updates when running on the `master` branch.

## How to run it

You need Git, Bash, curl, and an internet connection. On Windows, use Git Bash or WSL with access to PowerShell.

```bash
git clone https://github.com/BrandosFotos/tools.git
cd tools
bash main.sh
```

Enter the number for the option you want, or `0` to exit. Some installs may need administrator access. The macOS menu installs Homebrew if it is missing, and the Windows install scripts use Chocolatey.

## Files

- `main.sh` - Main menu and OS detection
- `mac/` - macOS install scripts
- `win/` - Windows PowerShell scripts
- `zshrc` - My shell settings

This is mostly for my own setup, so look through the scripts before using them. The macOS shell setup replaces your `.zshrc`, so back it up first if you want to keep it.
