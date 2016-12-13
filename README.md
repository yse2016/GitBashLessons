# GitBashLessons
Git Bashをはじめてインストールして使う際の導入レッスン。
yt@20161213


## Git Bash( Git for Windows )をインストールする.

1. [web site](https://git-for-windows.github.io/)にアクセスする.
2. インストーラをダウンロードする.
3. ↑を使って Git Bash をインストールする.
  - そのまま 'next' 'install'

## Git Bashをつかう

1. Explorerで、HomeDir( c:\Users\160xxx )を開く.
2. ↑ウィンドウを、画面の右半分に表示する.
3. Git Bashを起動する.
4. ↑ウィンドウを、画面の左半分に表示する.
5. Git Bashで、「現在のdirを確認」する.

  ```bash
  pwd
  ```

6. Git Bashで、「現在のdirにある file, dir のリストを表示」する.

  ```bash
  ls
  ```

7. Git Bashで、GitHubのdir( 160xxx > 20161213 )に移動する.

  ```bash
  cd documents
  cd github
  ls
  cd 160xxx
  ls
  cd 20161213
  ls
  ```

8. Git Bashで、Commit する.( 必要なときに実行してください )

  ```bash
  git status
  git add .
  git commit -m "ShowText.java updated."          <- 必要なコメントを書く.
  git status
  ```

9. Git Bashで、push( sync )する.( 必要なときに実行してください )

  ```bash
  git status
  git push origin master
  ```

10. Git Bashで、clone する.( 必要なときに実行してください )

  ```bash
  cd
  cd documents
  cd github
  pwd
  ls
  git clone https://github.com/YSE2016/GitHubLessons.git
  ls
  cd GitHubLessons
  ls
  ```

11. Git Bashで、masterブランチに、他のブランチ( testとか )を、merge(マージ)する.

  ```bash
  cd
  cd documents
  cd github
  cd 160136                <- リポジトリのdirに入る
  git branch
  git checkout master
  git merge test
  ls
  ```

12. Git Bashで、新しいブランチをつくる.

  ```bash
  cd
  cd documents
  cd github
  cd 160999               <-リポジトリのdirに入る
  git branch
  git checkout -b 新しいブランチ名
  git branch
  ```

end.
