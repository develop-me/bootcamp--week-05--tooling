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

## [Next level →](10-fin.md)