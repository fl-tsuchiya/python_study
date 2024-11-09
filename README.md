# Python学習メモ
Python一年生第2版を進める。
ただし、第1章Lesson2は無視して、かわりに下記の環境構築を行う。

## 環境構築

### 大まかな流れ

1. **Homebrew(ホームブリュー)** のインストール  
   ※HomebrewはmacOSのパッケージ管理システム

1. Homebrewを使って **Python(パイソン)** のインストール
    1. **tcl-tk** のインストール  
      ※tcl-tkはGUIアプリケーションを作成するためのツールキットもしくはAPI。pythonから使う場合はpythonインストール前にtcl-tkをインストールしておく必要がある

    1. **pyenv** のインストール  
      ※pyenvはpythonの仮想的な環境管理システム。pythonを複数バージョンインストールし、切り替えられるようにするツール

    1. pyenv から **python** のインストール
1. IDE(Integrated Development Environment: 統合開発環境)として **Visual Studio Code(ヴィジュアル スタジオ コード)** のインストール
   ※IDEとは、プログラミングコード記述を手助けしたり、コード実行を簡単に行えるアプリケーションのこと
      - Visual Studio Codeの入手とインストール
      - Visual Studio Codeの日本語化
      - Visual Studio Codeにpython拡張機能のインストール(ms-python)

### Homebrew(ホームブリュー)のインストール
1. ターミナルを開く
2. https://brew.sh/ja/ からインストール用コマンドをコピー、ターミナルに貼り付けて実行。するとインストール作業が始まる
3. 以下の画面の様にpasswordの入力が求められた場合、Macのログインパスワードを入力する
```
==> Checking for `sudo` access (which may request your password)...
Password:
```
4. 以下のメッセージがでたら、returnキーを押す
```
Press RETURN/ENTER to continue or any other key to abort:
```
5. `==> Installation successful!`とメッセージが出たら、インストールは完了。パスの設定と、実行できるか確認作業に移る
6. インストール完了メッセージの後に`==> Next steps`があるので、これにしたがって、パス設定のためのコマンド2行を1行ずつコピーしてターミナルで実行する。下記にコマンド例を示すが、必ず自分のインストール作業をしたターミナルに表示されているコマンドをコピーして実行すること
```
例 1行目：(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/<<Macのユーザー名>>/.zprofile
```
```
例 2行目：eval "$(/opt/homebrew/bin/brew shellenv)"
```
8. ターミナルで`brew help`と入力し、brewの使い方が表示されればインストール作業は完了となる

### Python(パイソン)のインストール

### Visual Studio Code(ヴィジュアル スタジオ コード)のインストール
