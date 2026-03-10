# Mac Dotfiles & Automation

An automated macOS development environment setup, optimized for a fast, portable transition between corporate machines. Inspired by Christoph Nakazawa's dotfiles.

Includes automated configurations for:

- **Zsh & Oh My Zsh** (with Powerlevel10k theme)
- **Homebrew** (Apps & CLI tools)
- **VS Code & Cursor** (Settings, Keybindings, and Extensions)
- **Fonts** (MesloLGS NF for terminal icons)

## 🛠 Installation on a New Mac

### 1. Authenticate with Git

Log in to GitHub and set up a new SSH key via GitHub → Settings → SSH and GPG Keys → New SSH key
<https://docs.github.com/en/authentication/connecting-to-github-with-ssh>

### 2. Clone the Repository

Clone this repository into your home directory:

```bash
git clone git@github.company.com:<username>/dotfiles.git ~/dotfiles
cd ~/dotfiles
```

### 3. Install

```
./homebrew
./bootstap
```

### 4. Maintenance

When you change a setting in VS Code/Cursor or update your .zshrc:
Make the change directly in the `~/dotfiles` directory.
Commit and push the changes.
If you install a new Homebrew package, update the Brewfile by running: `brew bundle dump --force --file=~/dotfiles/Brewfile`.
