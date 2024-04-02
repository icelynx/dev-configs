# Git notes

## Configs

```bash
# Identity
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
git config gpg.format ssh
git config user.signingKey ~/.ssh/id_rsa.pub

# Safer and easier history rewrite
git config --global rerere.enabled true
git config --global rerere.autoUpdate true
git config --global alias.fpush push --force-with-lease

# QoL
git config --global branch.sort -committerdate
git maintenance start
```

Can also use `--local` flag to write directory specific configuration.

## Commands

Diff by words, not just lines.

```bash
git diff --word-diff
```

Sign a push to remote

```bash
git push --signed
```