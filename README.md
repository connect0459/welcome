# 新歓ページ

タスクの軽いメモ

## ワイヤーフレーム

- [入部までの流れ (Figma)](https://www.figma.com/file/q4AYBpEXSH1MYNqlwRfFNB/omu.studyfortwo.org?type=design&t=1z9pLdd3CHPLbhD7-6)
- [一年間の活動・よくある質問 (Canva)](https://www.canva.com/design/DAF-6mgRsEE/Y0FDzGdhdTpwdLzzAEyeqw/edit)

## コード

### 管理方法

コードは Git で管理します。以下に Git のインストール～ GitHub のリポジトリに push する方法をまとめます。

1. **Gitのインストール**
    - <https://git-scm.com/download/win> からGitのWindowsバイナリをダウンロードします。
    - インストーラーを実行し、デフォルトの設定でインストールします。

2. **GitHubのアカウント作成**
    - <https://github.com/> にアクセスし、アカウントを作成します。

3. **SSHキーの生成**
    - コマンドプロンプトを開き、`ssh-keygen -t rsa -b 4096 -C "your_email@example.com"` と入力します。
    - 指示に従い、キーのパスフレーズを設定します。
    - `%UserProfile%\.ssh\id_rsa.pub` ファイルに公開鍵が生成されます。

4. **GitHubにSSHキーを登録**
    - GitHubへログインし、設定 > SSH and GPG keys より "New SSH key" をクリックします。
    - id_rsa.pub ファイルの内容をコピーし、キーのタイトルを入力して "Add SSH key" をクリックします。

5. **GitHubのアカウント設定**
    - `git config --global user.name "Your Name"` と入力し、名前を設定します。
    - `git config --global user.email "your_email@example.com"` と入力し、メールアドレスを設定します。

6. **リポジトリのクローン**  
    - クローンしたいリポジトリの `git@github.com:ユーザー名/リポジトリ名.git` のSSH URLをコピーします。
    - `git clone git@github.com:ユーザー名/リポジトリ名.git` と入力し、リポジトリをクローンします。

7. **ブランチの作成**
    - `git checkout -b #1_develop/coding` と入力し、新しい "1_develop/coding" ブランチを作成します。

8. **ファイルの編集**
    - お好みのテキストエディタでファイルを編集します。

9. **変更をコミット**
    - `git status` と入力し、変更されたファイルを確認します。
    - `git add .` と入力し、全ての変更をステージングします。
    - `git commit -m "コミットメッセージ"` と入力し、変更をコミットします。

10. **変更をプッシュ**
    - `git push origin #1_develop/coding` と入力し、"1_develop/coding"ブランチをGitHubにプッシュします。

11. **プルリクエストの作成**  
    - GitHubのリポジトリページへアクセスし、"Compare & pull request" ボタンを押します。
    - プルリクエストのタイトルと説明を入力し、"Create pull request" ボタンを押します。

12. **プルリクエストのマージ**
    - レビューが完了したら、"Merge pull request" ボタンを押し、変更をmainブランチにマージします。

### コーディング

以下の二つの拡張機能を Visual Studio Code にインストールしてください。

- [Live Sass Compiler](https://marketplace.visualstudio.com/items?itemName=glenn2223.live-sass)
- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

Live Sass Compiler は `.scss` ファイルを `.css` ファイルに変換する拡張機能です。 Live Server は `.html` ファイルをブラウザ上に公開し、リアルタイムで編集が反映される拡張機能です。
