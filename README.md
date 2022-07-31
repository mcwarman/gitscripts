# gitscripts

Works on both windows and mac. Add the directory to your path.

For windows if you're using post-git for tab completion add then add then as aliases:

```powershell
git config --global alias.clone-to-src clone-to-src
```

## Scripts

### `clone-to-source`

Takes git repo URL as argument and clones repo to `$HOME/code/src/<repo_url>/<org>/<repo>`.

```shell
git clone-to-src git@github.com:mcwarman/gitscripts.git
cd ~/code/src/github.com/mcwarman/gitscripts
```

### `dependabot-merge`

Creates a branch `dependabot-merge`, then attempts to rebase and merge all branches `origin/dependabot/...` into it.

### `gone`

Cleans branches no longer present on remote. `git gone --help` for more information.

### `switch-default`

Switch and update default branch, also runs `git gone -pD`.

### `whoami`

Returns configured `user.name` and `user.email`.
