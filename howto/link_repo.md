# リモートリポジトリとローカルリポジトリを関連付ける

## [方法1 (簡単)] リモートリポジトリをクローンしてファイルを追加する

```bash
$ git clone <remote repo url>
$ cd <リポジトリのフォルダ>
$ # ファイルを追加する
$ # git add する
$ # git commit する
$ # git push する
```

## [方法1 (少し複雑)] ローカルリポジトリをリモートリポジトリに関連付ける

```bash
$ cd <ローカルプロジェクトのフォルダ>
$ git init  # まだしてない場合
$ # git add する
$ # git commit する
$ git remote add origin <remote repo url>
$ git remote -v  # ちゃんとセットされているか確認
$ git pull  # リモート側にデータがある場合，ローカルに統合
$ git push
```