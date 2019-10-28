# Bonus Level: Configure Some Git Settings

## Configure Git to use VS Code as its editor

### Mac

In VS Code: `shift + ⌘ + P`

Type or paste `> Shell Command: Install 'Code' command in path` hit `[Enter]`

### Windows

In VS Code: `shift + ctrl + P`

Type or paste `> Shell Command: Install 'Code' command in path` hit `[Enter]`

Make sure you selected Add to PATH during the installation.

### All systems

From the command line, run

```bash
git config --global core.editor "code --wait"
```

## So that Git knows who your commits are made by

```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

## So that Git ignores unneccessary files

### Mac

We want to ignore `.DS_Store` files. These files are made by the Mac filesystem to store folder attributes, and are not part of our projects.

```bash
touch ~/.gitignore
cat ".DS_Store" > ~/.gitignore_global
cat "*.code-workspace" > ~/.gitignore_global
git config --global core.excludesfile ~/.gitignore_global
```

### Windows

In ConEmu:

```bash
touch ~/.gitignore
cat "Thumbs.db" > ~/.gitignore_global
cat "*.code-workspace" > ~/.gitignore_global
git config --global core.excludesfile ~/.gitignore_global
```

## [Next level →](10-fin.md)