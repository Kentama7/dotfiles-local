# dotfiles-local

# Requirements

- zsh
- [peco](https://github.com/peco/peco)
- [ghq](https://github.com/x-motemen/ghq)

# Setup

## .env

```shell
vim ~/.env
```

```
GITHUB_TOKEN=xxxxxxxx
```

## dotfiles

https://github.com/Kentama7/dotfiles

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

Set `ZSH_THEME="typewritten"` in `.zshrc.local` file.

### Plugins

- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)   
  ```
  git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
  ```
- [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)   
  ```
  git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
  ```
- [history-substring-search](https://github.com/zsh-users/zsh-history-substring-search)   
  ```
  git clone https://github.com/zsh-users/zsh-history-substring-search ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-history-substring-search
  ```
- [enhancd](https://github.com/b4b4r07/enhancd)   
  ```
  git clone https://github.com/b4b4r07/enhancd ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/enhancd
  ```

