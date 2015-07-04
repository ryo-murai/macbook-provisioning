# macbook-provisioning

## how to run

### preparation
#### XCode
``` sh
sudo xcodebuild -license
```

#### Homebrew
``` sh
xcode-select --install ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

brew doctor

brew update
```

#### Ansible
``` sh
brew install ansible
```

### run playbook

``` sh
HOMEBREW_CASK_OPTS="--appdir=/Applications" ansible-playbook -i hosts -vv localhost.yml
```



## 参考にさせて頂いたもの
- [t-wadaのブログ -- Mac の開発環境構築を自動化する (2015 年初旬編)](http://t-wada.hatenablog.jp/entry/mac-provisioning-by-ansible)
 - ほぼパクらせて頂いた
