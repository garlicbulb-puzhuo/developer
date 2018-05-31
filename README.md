# Developer Notes

### Environment setup

#### mac setup

* http://sourabhbajaj.com/mac-setup/

#### 如何配置一个高效的mac工作环境

* https://github.com/macdao/ocds-guide-to-setting-up-mac

### oh-my-zsh setup

* main repo: https://github.com/robbyrussell/oh-my-zsh

* Related dependencies
  * https://github.com/powerline/fonts
  
     Remember to restart your iTerm app after installation
  
  * http://ethanschoonover.com/solarized
  * https://github.com/powerline/powerline
  * https://github.com/vim-airline/vim-airline

### Useful documents and tips

#### Vagrant

* https://medium.com/@JohnFoderaro/how-to-set-up-a-local-linux-environment-with-vagrant-163f0ba4da77

#### Cheatsheets

* markdown: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

#### Useful git aliases

```
[alias]
    squash = "!f(){ CUR=`git rev-parse HEAD` && git reset --soft ${1} && git commit -m \"$(git log --format=%B ${1}..${CUR})\"; };f"
    pub = "!f() { git push -u ${1:-origin} HEAD:`git config branch.$(git name-rev --name-only HEAD).merge | sed -e 's@refs/heads/@refs/for/@'`; }; f"
    pretty=log --oneline --abbrev-commit --all --graph --decorate --color
```

#### brew

* [Install a specific version in brew](http://stackoverflow.com/questions/3987683/homebrew-install-specific-version-of-formula)
