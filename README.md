# Mac Setup Instructions

The instructions to setup dev environment on a new a Mac. Please feel free to use it if your setup looks similar.

> Note: Below instructions are applicable only for macOS

## 1. Setting up Terminal

#### 1. Install [oh-my-zsh](https://ohmyz.sh/)

```
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

#### 2. Install following Zsh plugins:

- [Zsh Autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
  ```
  git clone https:://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
  ```
- [Zsh Syntax Highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
  ```
  git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
  ```
  **Note:** Setup of above plugins in `.zshrc` will be automatically done in later steps when we install your DotFiles setup.

#### 3. Download [Hyper.js](https://hyper.is/) terminal. :pray:

#### 4. Install following plugins for Hyper.js:

- [hyper-snazzy](https://github.com/sindresorhus/hyper-snazzy)
- [hypercwd](https://github.com/hharnisc/hypercwd)
  **Note:** Just open `~/.hyper.js` file and add above in list of plugins field like below:

```
plugins: [ 'hypercwd','hyper-snazzy'],
```

> Note: Below 2 steps can be skipped as this involves a private repo

#### 5. Clone [DotFiles repo](https://github.com/punitda/DotFiles)

#### 6. Run symlink setup scripts in DotFiles folder and done. :metal:

#### 7. Copy .zsh_history file from your old machine

This will contain history of all the commands you typed on your old machine. Copy it to $HOME folder.

<br />

## 2. Installing dependencies

#### 1. Install HomeBrew

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

#### 2. Install Git

```sh
brew install git
```

#### 3. Install JDK

```sh
# JDK 11
brew install openjdk@11

# JDK 17
brew install openjdk@17
```

#### 4. Install Nvm (For managing Node versions)

```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
```

#### 5. Install rbenv (For managing Ruby versions)

```sh
brew install rbenv ruby-build
```

#### 5. Install Fvm (For managing Flutter versions)

```sh
brew tap leoafarias/fvm
brew install fvm
```
