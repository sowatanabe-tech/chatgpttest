# プロフィールサイト

このリポジトリには、Bootstrap を用いて装飾したシンプルな個人プロフィールサイトのテンプレートが含まれています。`index.html` のテキストを書き換えるだけで、名前や職種、経歴などの基本情報を公開できます。

## 使い方

1. `index.html` を開き、名前や自己紹介、経歴、リンクなどをあなた自身の内容に編集します。
2. 変更内容をコミットして GitHub にプッシュすると、GitHub Pages などの静的ホスティングでそのまま公開できます。
3. Bootstrap のクラスを変更することで、レイアウトやカラーを簡単に調整できます。

## プレビュー

### ローカルで確認する

ローカルでプレビューするには、任意の静的サーバーを使用してください。例えば Python をお使いの場合は以下のコマンドで起動できます。

```bash
python -m http.server
```

その後、ブラウザで <http://localhost:8000> を開くとサイトを確認できます。HTML ファイルを直接ブラウザにドラッグ＆ドロップするだけでも簡易表示できますが、Bootstrap の一部機能が読み込めない場合があるため、サーバー経由のプレビューをおすすめします。

### GitHub Pages で確認する

1. GitHub のリポジトリページで **Settings** → **Pages** に移動します。
2. **Build and deployment** の **Source** で「Deploy from a branch」を選択します。
3. **Branch** に `main`（または公開したいブランチ）と `/ (root)` を指定して **Save** します。
4. 数分後に表示される公開 URL へアクセスすると、GitHub 上でも完成したプロフィールサイトを確認できます。

## GitHub へ反映する手順

リポジトリを手元で編集した後、次のコマンドで変更を GitHub に反映できます。

```bash
# 最新の変更を取り込む
git pull

# 変更したファイルをステージしてコミット
git add index.html README.md
git commit -m "Update profile content"

# GitHub へプッシュ
git push
```

GitHub Actions や GitHub Pages を利用している場合は、プッシュ後に自動でサイトが公開されます。
