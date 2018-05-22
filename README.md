# raspi
Setup raspberry pi

# 準備
## piユーザのパスワード設定
1. `sudo raspi-config` → 1.Change User Password

## ssh,vncの有効化
1. メニュー→設定→Raspberry Piの設定→SSH、VNCを有効
1. `sudo shutdown -r now`
1. PCからRasPiにssh接続、vnc接続できることを確認

# githubへのssh接続設定
1. `cd ~/.ssh`
1. `ssh-keygen -t rsa -C [your mail address]`
1. `chmod 600 id_rsa*`
1. githubの画面を開く
1. SSH and GPG keys→New SSH keyから、id_rsa.pubの内容を設定

# githubの登録
1. `git config --global user.email "[your mail address]"`
1. `git config --global user.name "[your user name]"`

