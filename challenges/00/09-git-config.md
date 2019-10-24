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
git config --global --edit
```

Then edit values as required, uncomment (remove `#`).

Good starting point:

```
[user]
	name = Your Name
	email = you@email.com
[push]
	default = matching
```

Then, to save and exit.

## [Next level →](10-fin.md)