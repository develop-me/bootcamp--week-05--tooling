# Level 7: Generate SSH keys

You'll need to generate a new keypair using [GitHub's suggested process](https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent):

```bash
$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

Replace `your_email@example.com` with your own email or comment.

Hit `[Enter]` at all the prompts.

Then, once you've finished creating your keys, output the public part of the key with:

```bash
$ cat ~/.ssh/id_rsa.pub
```

## [Next level →](08-add-ssh-github.md)