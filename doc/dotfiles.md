# dotfiles

https://qiita.com/yutakatay/items/c6c7584d9795799ee164


## zsh

### aliasの設定時の注意

#### 不要なコマンドが起動時に呼ばれてしまう

`alias ls="ls -l $(find /)"`
などのようにでサブシェル実行しない

起動時に呼ばれてしまい起動が遅くなる

`alias ls='ls -l $(find /)'`
シングルクオートなら起動時に実行されないですむ

https://stackoverflow.com/questions/47211413/zsh-alias-with-command-parameter