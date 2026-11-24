# Dotfiles

Personal dotfiles repository containing configurations for **Hyprland**, **Quickshell**, and other interconnected applications required to run my complete Linux desktop environment.

## Installation

Since Git cannot clone a repository directly into a non-empty directory, the easiest way to install these dotfiles is to clone the repository into a temporary location and copy its contents to `~/.config`.

### 1. Clone the repository

```bash
git clone git@github.com:QuantumKoga/dotfiles.git /tmp/dotfiles
```

### 2. Copy configurations

Copy the repository contents into your existing `~/.config` directory:

```bash
cp -a /tmp/dotfiles/. ~/.config/
```

This will overwrite existing files with matching names while preserving unrelated configurations.

**Note:** If a file in your existing `~/.config` conflicts with a directory in the repository (or vice versa), remove the conflicting file or directory before copying.

### 3. Clean up

Once the files have been copied successfully, remove the temporary clone:

```bash
rm -rf /tmp/dotfiles
```

### 4. Verify the installation

The repository's `.git` directory is copied along with the configuration files, allowing you to manage your dotfiles directly from `~/.config`.

```bash
cd ~/.config
git status
git remote -v
```

You can now manage your dotfiles using regular Git commands.

## Managing Dotfiles

All Git operations can be performed directly from `~/.config`:

```bash
git status
git add .
git commit -m "Update dotfiles"
git push
git pull
```

