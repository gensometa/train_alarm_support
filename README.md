# 乗換アラーム - GitHub Pages

このディレクトリには、GitHub Pagesで公開するサポートページとプライバシーポリシーが含まれています。

## ファイル構成

- `support.html` - アプリのサポートページ（よくある質問、お問い合わせ先など）
- `privacy.html` - プライバシーポリシー

## GitHub Pagesでの公開手順

### 1. GitHubリポジトリを作成（未作成の場合）

```bash
# リポジトリを初期化（まだの場合）
cd /Users/po/Documents/claude/train_alerm
git init

# 最初のコミット
git add .
git commit -m "Initial commit"

# GitHubにプッシュ
git remote add origin https://github.com/[ユーザー名]/train_alarm.git
git branch -M main
git push -u origin main
```

### 2. GitHub Pagesを有効化

1. GitHubのリポジトリページにアクセス
2. `Settings` タブをクリック
3. 左サイドバーの `Pages` をクリック
4. `Source` で `Deploy from a branch` を選択
5. `Branch` で `main` ブランチと `/docs` フォルダーを選択
6. `Save` をクリック

### 3. 公開URLを確認

数分後、以下のURLでアクセスできるようになります：

```
https://[ユーザー名].github.io/train_alarm/support.html
```

このURLをApp Store Connectの「サポートURL」に設定してください。

## App Store Connect での設定

### サポートURL
```
https://[ユーザー名].github.io/train_alarm/support.html
```

### プライバシーポリシーURL（必要な場合）
```
https://[ユーザー名].github.io/train_alarm/privacy.html
```

## カスタマイズ

### メールアドレスの変更

両方のHTMLファイル内の以下の部分を実際のメールアドレスに変更してください：

```html
<a href="mailto:support@example.com">support@example.com</a>
```

↓

```html
<a href="mailto:your-email@example.com">your-email@example.com</a>
```

### デザインのカスタマイズ

`<style>` タグ内のCSSを編集することで、色やレイアウトを変更できます。

主要なカラーコード：
- メインカラー（紫）: `#667eea`
- アクセントカラー（濃い紫）: `#764ba2`

## 注意事項

- HTMLファイルを更新した場合、GitHubにプッシュするとGitHub Pagesに自動反映されます
- 反映には数分かかる場合があります
- リポジトリを公開（Public）にする必要があります（Private リポジトリでは GitHub Pages は有料プランが必要）
