# Git環境の構築

必要に応じて[Git Documentation](https://git-scm.com/doc)を確認することを勧める．

## Windows

[Git公式サイト](https://git-for-windows.github.io/)にアクセスし，インストーラをダウンロードする

インストーラを起動し，インストールを開始する．

設定は好みで．ただし，デフォルトエディタは初期設定だとVimになっているので，慣れていない人は変えたほうがよい(Nano, Notepadなど)．

[初期設定へ](#初期設定)

## Linux

Gitをインストールする

```bash
$ sudo apt install git-all  # Debian/Ubuntu
$ sudo yum install git-all  # Fedora
```

[初期設定へ](#初期設定)

## 初期設定

`git config`の設定をする必要がある．

特に，`user.name`と`user.email`は設定されていないとGitの様々な機能が使えなくなる．

Gitの設定ファイルは以下の3種類があるが，基本的には`global`を設定すればよい．
- `system`: システム全体(全ユーザ)の設定
- `global`: 現在のユーザの設定
- `local`: 現在のリポジトリの設定

(例)
```bash
$ git config --global user.name fujinolab
$ git config --global user.name ri0000xx@ed.ritsumei.ac.jp
```

設定された値を確認するには以下のコマンドが使用できる．

(例)
```bash
$ git config -l
user.name=fujinolab
user.email=ri0000xx@ed.ritsumei.ac.jp
```