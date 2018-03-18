# setup-macos
[![Build Status](https://travis-ci.org/ioapm/setup-macos.svg?branch=master)](https://travis-ci.org/ioapm/setup-macos)

Setup my macbook.

## Getting started

### Install Xcode
```
xcode-select --install
sudo xcode-select --switch /Library/Developer/CommandLineTools/
```

### Install Homebrew & Ansible
```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew install ansible && brew doctor
```

### Setup my macbook
```
git clone git@github.com:ioapm/setup-macos.git
cd setup-macos
ansible-playbook setup.yml -vv -i hosts
```