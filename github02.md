コピー＆ペーストするだけで使えるように、Markdown形式で整理しました。

-----

### GitHubでファイルをWeb管理する手順

この手順に従えば、VS Codeで作成したMarkdownファイルをGitHubにアップロードし、Web上で管理できるようになります。

-----

### 1\. GitHubでの準備

GitHubにログインし、新しいリポジトリを作成します。

1.  GitHubのウェブサイトで、右上の **`+`** ボタンから **`New repository`** を選択。
2.  リポジトリ名（例: `my-commands`）を入力。
3.  **`Add a README file`** にチェックを入れて、 **`Create repository`** をクリック。

-----

### 2\. ローカルでの作業

VS Codeで、このページの内容を新しいファイルに貼り付けて保存します。

  * **ファイル名**: `Git-Bash-Commands.md`など、分かりやすい名前をつけましょう。

-----

### 3\. Git Bashでのアップロード

Git Bashを開き、以下のコマンドを順番に実行します。

1.  **リポジトリをクローン**
    GitHubで作成したリポジトリのURLをコピーし、ローカルにクローンします。

    ```bash
    git clone https://github.com/your-username/your-repository-name.git
    ```

2.  **フォルダに移動**
    クローンしてできたリポジトリのフォルダに移動します。

    ```bash
    cd your-repository-name
    ```

3.  **ファイルを移動**
    先ほどVS Codeで作成した `.md` ファイルを、このフォルダの中に移動させます。

4.  **変更をコミット**
    ファイルを追加し、コミットします。

    ```bash
    git add .
    git commit -m "変更を更新"
    ```

5.  **GitHubへプッシュ**
    最後に、変更内容をGitHubに送信します。

    ```bash
    git push
    ```

これで、GitHubのリポジトリに `.md` ファイルがアップロードされ、Webブラウザで内容を閲覧・管理