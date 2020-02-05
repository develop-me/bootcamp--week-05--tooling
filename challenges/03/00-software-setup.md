# Check that you have node, npm and gulp installed:

## Run `node -v`

Expect something like:

```bash
v12.10.0
```

Else run:

### Mac

```bash
brew install node
```

### Windows

```bash
curl -sL "https://deb.nodesource.com/setup_12.x" | sudo -E bash -
sudo apt-get install -y gcc make ruby ruby-dev
sudo apt-get install -y nodejs
```

## Run `npm -v`

Expect something like:

```bash
6.13.4
```

## Run `gulp -v`

Expect something like:

```bash
CLI version: 2.2.0
Local version 3.9.1 (or might be Unknown)
```

Else run:

```bash
npm install gulp-cli -g
npm install gulp -D
```

*Note: you may need to add `sudo` before each command if they fail due to permissions.*
