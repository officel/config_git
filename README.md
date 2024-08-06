# config_git

my git config on $XDG_CONFIG_HOME/git/

## usage

```bash
cd ~/.config  # $XDG_CONFIG_HOME or $HOME/.config
git clone https://github.com/officel/config_git.git ./git

# or I do it this way
cd ~/repos/github.com/officel/
git clone https://github.com/officel/config_git.git
ln -s ~/repos/github.com/officel/config_git/ ~/.config/git
```

- install id_rsa (manual)
- fix git config remote.origin.url after clone

## see

- https://git-scm.com/docs/git-config
- https://github.com/github/gitignore
- https://www.conventionalcommits.org/
- https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html

# related my projects

- [officel/config_aqua: .config/aqua](https://github.com/officel/config_aqua)
- [officel/config_bash: .config/bash](https://github.com/officel/config_bash)
- [officel/config_git: .config/git](https://github.com/officel/config_git)

# note

## ローカルリポジトリだけ ignore

- チームでは ignore しないが、個人では ignore したい
- 個人の共通設定（このリポジトリの ignore のように）では ignore しないが、特定のリポジトリでは ignore したい
- （リポジトリの）`.git/info/exclude` に追加
