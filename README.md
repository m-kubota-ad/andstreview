# andST Review 2025

GitHub Pagesで公開するための手順

## GitHub Pagesで公開する手順

### 1. GitHubでリポジトリを作成

1. [GitHub](https://github.com)にログイン
2. 右上の「+」→「New repository」をクリック
3. リポジトリ名を入力（例: `andstreview`）
4. 「Public」を選択
5. 「Initialize this repository with a README」は**チェックしない**（既にローカルにファイルがあるため）
6. 「Create repository」をクリック

### 2. リモートリポジトリを追加してプッシュ

GitHubでリポジトリを作成したら、表示されるURL（例: `https://github.com/ユーザー名/andstreview.git`）を使って、以下のコマンドを実行してください：

```bash
git remote add origin https://github.com/ユーザー名/andstreview.git
git branch -M main
git push -u origin main
```

### 3. GitHub Pagesを有効化

1. GitHubリポジトリのページで「Settings」タブをクリック
2. 左メニューから「Pages」を選択
3. 「Source」で「Deploy from a branch」を選択
4. 「Branch」で「main」を選択し、「/ (root)」を選択
5. 「Save」をクリック

### 4. 公開URLの確認

数分後、以下のURLでサイトにアクセスできます：
- `https://ユーザー名.github.io/andstreview/`

または、Settings > Pages ページで公開URLが表示されます。

## ローカルでの確認

ブラウザで `index.html` を直接開くか、ローカルサーバーで確認できます：

```bash
# Python 3の場合
python -m http.server 8000

# Node.jsの場合（http-serverが必要）
npx http-server
```

その後、ブラウザで `http://localhost:8000` にアクセスしてください。

