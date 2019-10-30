# Check that you have node, npm and gulp installed:

## Run `node -v`

Expect something like:

```bash
v12.10.0
```

Else run:

### Mac

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
6.12.0
```

## Run `gulp -v`

Expect something like:

```bash
[09:44:18] CLI version 1.4.0
[09:44:18] Local version 3.9.1
```

Else run:

```bash
npm install gulp-cli -g
npm install gulp -D
```

*Note: you may need to add `sudo` before each command if they fail due to permissions.*