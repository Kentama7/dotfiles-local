# dotfiles-local

# 事前準備

## dotfiles

```shell
git clone https://github.com/Kentama7/dotfiles.git ~/dotfiles
brew tap thoughtbot/formulae
brew install rcm
env RCRC=$HOME/dotfiles/rcrc rcup
```
## dotfiles-local

```shell
git clone https://github.com/Kentama7/dotfiles-local.git ~/dotfiles-local
```

## oh-my-zh

```shell
git clone https://github.com/ohmyzsh/ohmyzsh.git ~/.oh-my-zsh
cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc.local
```

### Theme

https://typewritten.dev/

```shell
git clone https://github.com/reobin/typewritten.git $ZSH_CUSTOM/themes/typewritten
ln -s "$ZSH_CUSTOM/themes/typewritten/typewritten.zsh-theme" "$ZSH_CUSTOM/themes/typewritten.zsh-theme"
ln -s "$ZSH_CUSTOM/themes/typewritten/async.zsh" "$ZSH_CUSTOM/themes/async"
```

### Plugins

- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

