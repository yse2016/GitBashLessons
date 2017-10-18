# GitBashLessons
Git Bashをはじめてインストールして使う際の導入レッスン。
yt@20161213, 20171017


## Git Bash( Git for Windows )をインストールする.

1. [web site](https://git-for-windows.github.io/)にアクセスする.
2. インストーラをダウンロードする.
3. ↑を使って Git Bash をインストールする.
  - そのまま 'next' 'install'

## Git Bashをつかう

目的は、ファイル・フォルダ（ディレクトリ; directory）の操作を経験してGitBashに慣れること。

MacユーザはGitBashの代わりに「terminal」を使用してください。

WindowsPCでの個人フォルダ( HomeDir; ホームディレクトリ )が次の場所にあるとします。もちろん実際にはユーザ名もフォルダ名も異なると思います。適当に読み替えてください。

`c:\Users\170xxx`

1. エクスプローラ( Explorer )で、HomeDir( c:\Users\170xxx )を開く.
2. ↑ウィンドウを、画面の右半分に表示する.
3. Git Bashを起動する.
4. ↑ウィンドウを、画面の左半分に表示する.
5. Git Bashで、「現在のdirを確認」する.

  ```bash
  pwd
  ```

  ↑ExplorerとGit Bash両方とも同じHomeDirにアクセスしていることを確認します。

6. Git Bashで、「現在のdirにある file, dir のリストを表示」する.

  ```bash
  ls
  ```

  ↑わりとたくさん表示されます。ふだん表示されないものもあります。それらは「隠しフォルダ」です。ExplorerとGit Bashで共通しているものを探します。同じHomeDirにアクセスしていると実感します。

  次にファイルやdir（ディレクトリ=フォルダ）を操作します。

7. 新しいdirを作成し、その中に入る（そのdirを開く; そのdirにアクセスする）。

  Git Bashで次のコマンドを打ち込み enterキー を押下してください。"test4bash"という名前のdirができます。

  Git Bash等、コマンドで操作する時はいつも最後に enterキー を打って実行させます。

  ```bash
  mkdir test4bash
  ```

  Explorerのウィンドウに"test4bash"が出現したことを確認してください。

  Git Bashでも"test4bash"を確認しましょう。`ls`コマンドを実行します。

  ```bash
  ls
  ```

  以下、同様にコマンド操作の結果をGit BashでもExplorerでも確認します。

  注)."<- 〜"はコマンドの説明です。読むだけにして、入力しないでください。

  ```bash
  cd test4bash        <- test4bashに移動する
  pwd           <- 現在のdirを確認する
  ```

  Explorerでも"test4bash"フォルダをダブルクリックして開きます。


8. ファイルを作成・コピー・移動・削除する

  ファイルを一つ作成し、コピーして２つにします。

  ```bash
  touch test.doc      <- test.docというファイルを作る
  ls
  cp test.doc  test2.doc    <- test.docをコピーしてtest2.docを作る
  ls
  ```

  新しいdirを作成し、その中にファイルを一つ移動させます。

  ```bash
  mkdir docDir
  ls
  mv test2.doc docDir     <- test2.docを、docDirの中に移動(move)させる
  ls
  ls docDir       <- docDirの中にあるファイルを表示させる
  rm test.doc     <- test.docを削除(remove)する
  ls
  rm docDir/test2.doc     <- docDirの中のtest2.docを削除する
  ls docDir
  ls
  rmdir docDir    <- docDirを削除する(remove directory)
  ```


9. Git Bashを終了する

  作成したdirを削除して、Git Bashを終了します。

  ```bash
  cd ..             <- ひとつ上のdir（HomeDirのはず）に移動する
  rmdir test4bash
  ls
  exit        <- Git Bashを終了させる

  ```


とりあえず、ここまで。

基本的なコマンドを練習するためのメニューを追加する予定です。yt@20171017

end.
