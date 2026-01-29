# GitHub Pagesでの公開手順

このガイドでは、FAQページをGitHub Pagesで公開する手順を説明します。

## 📋 必要なもの

- GitHubアカウント（無料）
- Webブラウザ

## 🚀 公開手順

### ステップ1: GitHubアカウントの作成（既にある場合はスキップ）

1. https://github.com/ にアクセス
2. 「Sign up」をクリック
3. メールアドレス、パスワード、ユーザー名を入力
4. 認証手続きを完了

### ステップ2: 新規リポジトリの作成

1. GitHubにログイン
2. 右上の「+」アイコンをクリック → 「New repository」を選択
3. リポジトリの設定:
   - **Repository name**: `cosmotalk-faq` （任意の名前でOK）
   - **Description**: `コスモトークFAQページ` （省略可）
   - **Public** を選択（無料でGitHub Pagesを使用するため）
   - **Add a README file** のチェックは外す
4. 「Create repository」をクリック

### ステップ3: ファイルのアップロード

#### 方法A: Webインターフェースでアップロード（簡単）

1. 作成したリポジトリページで「uploading an existing file」をクリック
2. 以下のファイルをドラッグ&ドロップ:
   - `index.html`
   - `README.md`
3. 下部の「Commit changes」をクリック

#### 方法B: Git コマンドライン（上級者向け）

```bash
git clone https://github.com/[ユーザー名]/cosmotalk-faq.git
cd cosmotalk-faq
# index.html と README.md をコピー
git add .
git commit -m "Initial commit: Add FAQ page"
git push origin main
```

### ステップ4: GitHub Pagesの有効化

1. リポジトリページで「Settings」タブをクリック
2. 左メニューから「Pages」を選択
3. **Source** セクションで:
   - Branch: `main` を選択
   - Folder: `/ (root)` を選択
4. 「Save」をクリック
5. 数分待つと、ページ上部に公開URLが表示されます:
   ```
   Your site is live at https://[ユーザー名].github.io/cosmotalk-faq/
   ```

### ステップ5: 確認

表示されたURLにアクセスして、FAQページが正しく表示されることを確認してください。

⚠️ 初回公開は最大10分程度かかる場合があります。

## 🔄 ページの更新方法

### Webインターフェースで更新

1. リポジトリページで `index.html` をクリック
2. 右上の鉛筆アイコン（Edit this file）をクリック
3. 内容を編集
4. 下部の「Commit changes」をクリック
5. 数分後、公開ページに反映されます

### ローカルで編集してアップロード

1. `index.html` をダウンロード
2. テキストエディタで編集
3. リポジトリページで該当ファイルをクリック
4. 「Upload files」から更新版をアップロード

## 🌐 独自ドメインの設定（オプション）

既に独自ドメインをお持ちの場合:

1. Settings → Pages → Custom domain に独自ドメインを入力
2. DNSレコードを設定（詳細はGitHub公式ドキュメント参照）

## 📞 サポート

問題が発生した場合は、以下にご連絡ください:
- Mail: info@butaifarm.com
- TEL: 022-289-6768

## 📚 参考リンク

- [GitHub Pages公式ドキュメント](https://docs.github.com/ja/pages)
- [GitHub入門ガイド](https://docs.github.com/ja/get-started)
