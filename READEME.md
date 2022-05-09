# PID1-Ubuntu-on-WSL

## 概要

デフォルトでWSL2上では、`PID 1`を使用する`systemctl`等のコマンドが使用できない。  
しかし、WSL環境をStoreからダウンロードかつ、  
`wsl-systemd`を実行し、ubuntu{version}.exeから起動した場合は使用可能である。  
そこで、このリポジトリにて`wsl-systemd`の実行を起動時に行う処理を追加する。

ちょっとしたメモ程度である。

# セットアップ手順

1. StoreからWSLディストリビューションをダウンロード&インストールする。
1. インストールしたWSL環境に入る。
1. `sh ./setup.sh`を実行する。
1. Host側で`wsl --shutdown`をする。
1. `ubuntu{version}.exe`を実行してWSL環境に入る
