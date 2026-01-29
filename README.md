# コスモトーク FAQ ページ

IP無線機「コスモトーク」の顧客向けFAQページです。

## 📋 概要

このリポジトリは、株式会社舞台ファームが提供するIP無線機「コスモトーク」のよくある質問（FAQ）ページを管理しています。

## 🌐 公開URL

公開後のURL: `https://[あなたのGitHubユーザー名].github.io/[リポジトリ名]/`

## 📝 FAQの更新方法

### 質問と回答を追加する場合

1. `index.html` ファイルを開きます
2. 追加したいカテゴリーセクションを探します（例: `<!-- 使用方法 -->`）
3. 以下のコードをコピーして、該当セクション内に貼り付けます:

```html
<div class="faq-item">
    <div class="faq-question" onclick="toggleFaq(this)">
        <span class="faq-question-text">ここに質問を入力</span>
        <span class="faq-icon">▼</span>
    </div>
    <div class="faq-answer">
        <div class="faq-answer-content">
            ここに回答を入力
        </div>
    </div>
</div>
```

4. 「ここに質問を入力」と「ここに回答を入力」を実際の内容に変更
5. ファイルを保存してコミット

### 新しいカテゴリーを追加する場合

```html
<div class="category-section">
    <h3 class="category-title">カテゴリー名</h3>
    <!-- ここにfaq-itemを追加 -->
</div>
```

### 既存の質問を削除する場合

該当する `<div class="faq-item">...</div>` ブロック全体を削除します。

## 🎨 デザインのカスタマイズ

### 色の変更

`index.html` の `<style>` セクション内の `:root` 変数を編集します:

```css
:root {
    --primary-color: #1a7a8e;      /* メインカラー */
    --accent-color: #FFD700;        /* アクセントカラー */
    /* ... */
}
```

## 📞 お問い合わせ

株式会社舞台ファーム
- TEL: 022-289-6768
- Mail: info@butaifarm.com
- Web: https://butaifarm.com

## 📄 ライセンス

Copyright © 2025 株式会社舞台ファーム All Rights Reserved.
