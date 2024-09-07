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

- [Git - git-config Documentation](https://git-scm.com/docs/git-config)
- [GitAlias/gitalias: Git alias commands for faster easier version control](https://github.com/GitAlias/gitalias)
- [github/gitignore: A collection of useful .gitignore templates](https://github.com/github/gitignore)
- [Conventional Commits](https://www.conventionalcommits.org/)
- [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/latest/)

# related my projects

- [officel/config_aqua: .config/aqua](https://github.com/officel/config_aqua)
- [officel/config_bash: .config/bash](https://github.com/officel/config_bash)
- [officel/config_git: .config/git](https://github.com/officel/config_git)

# note

## ローカルリポジトリだけ ignore

- チームでは ignore しないが、個人では ignore したい
- 個人の共通設定（このリポジトリの ignore のように）では ignore しないが、特定のリポジトリでは ignore したい
- （リポジトリの）`.git/info/exclude` に追加
