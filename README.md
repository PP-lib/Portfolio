
# ポートフォリオサイト README

## 概要
このポートフォリオサイトは、技術記事、プロジェクト、画像などの視覚的要素を公開するために設計されています。
メインページ、記事ディレクトリ、および静的アセット（画像やスタイルシート）で構成されています。

## ディレクトリ構造
```
Portfolio/
│
├── index.html          # サイトのメインエントリーポイント
├── style.css           # サイト全体のスタイルシート
├── images/             # 画像アセットを格納するディレクトリ
├── articles/           # 各記事ファイルを格納するディレクトリ
│   ├── article1.html   # HTML形式のサンプル記事
│   ├── article2.md     # Markdown形式のサンプル記事
│   ├── style.css       # 記事専用のスタイルシート（オプション）
│   └── ...             # その他の記事
├── README.md           # このファイル（サイトの構造とルールを説明）
└── .git/               # Gitリポジトリのディレクトリ
```

## 記事執筆ガイドライン

### 1. ファイル形式
- 記事は **Markdown** または **HTML** 形式で記述してください。
- Markdownファイルには `.md` 拡張子を、HTMLファイルには `.html` 拡張子を使用してください。

### 2. メタデータ
各記事の識別と表示のために、以下の形式でメタデータを追加してください。Markdownの場合：

```markdown
---
title: "記事のタイトル"
author: "執筆者の名前"
date: "YYYY-MM-DD"
tags: ["タグ1", "タグ2"]
---
```

HTMLの場合は、以下のように `<head>` セクションに `<meta>` タグを記述してください：

```html
<head>
    <meta name="title" content="記事のタイトル">
    <meta name="author" content="執筆者の名前">
    <meta name="date" content="YYYY-MM-DD">
    <meta name="tags" content="タグ1, タグ2">
</head>
```

### 3. コンテンツ構成
- **イントロダクション**：記事の概要や目的を簡単に説明してください。
- **メインボディ**：適切な見出し（HTMLでは `<h1>` や `<h2>`、Markdownでは `#` や `##` を使用）でセクション分けしてください。
- **結論**：重要なポイントの要約や次のステップを示してください。

### 4. スタイルとメディア
- コンテンツを補完するために、必要に応じて画像を使用してください。画像は `images/` ディレクトリに配置してください。
- 画像の参照は相対パス（例：`../images/image1.png`）を使用してください。
- HTMLでは `<style>` ブロック、Markdownではインラインスタイルを使用してカスタムデザインを適用できます。

## スタイルとアクセシビリティ
- 見出しや段落のスタイルを統一してください。
- カラーコントラストを確保し、アクセシビリティに配慮してください。
- すべての画像に `alt` 属性を付与してください。

## コントリビューションガイド
- リポジトリをクローンし、変更用のブランチを作成してください。
- プルリクエストを通じて更新内容を提出してください。
- 記事構成およびガイドラインに従ってください。

---
このドキュメントはプロジェクトの進行に合わせて更新してください！


## 最新テンプレート

### HTMLテンプレート
```html
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="title" content="記事のタイトル">
    <meta name="author" content="執筆者の名前">
    <meta name="date" content="YYYY-MM-DD">
    <meta name="tags" content="技術, トレンド, プログラミング">
    <meta name="description" content="この記事では、最新の技術トレンドについて解説します。">
    <title>記事のタイトル | ポートフォリオ</title>
    <link rel="stylesheet" href="../style.css">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="../index.html">ホーム</a></li>
                <li><a href="#content">記事内容</a></li>
                <li><a href="../articles">他の記事</a></li>
            </ul>
        </nav>
    </header>

    <main id="content">
        <article>
            <header>
                <h1>記事のタイトル</h1>
                <p><strong>執筆者:</strong> 執筆者の名前 | <strong>公開日:</strong> YYYY-MM-DD</p>
            </header>

            <section>
                <h2>イントロダクション</h2>
                <p>この記事では、最新の技術トレンドや注目ポイントについて解説します。</p>
            </section>

            <section>
                <h2>主題: 最新トレンド</h2>
                <p>ここで、技術の背景、動向、具体的な事例などを解説します。</p>
                <ul>
                    <li>例: AIの進化とその応用</li>
                    <li>例: Web3の可能性</li>
                    <li>例: サステイナブルな開発手法</li>
                </ul>
            </section>

            <section>
                <h2>結論</h2>
                <p>トピックの要約や、今後の方向性について述べます。</p>
            </section>
        </article>
    </main>

    <footer>
        <p>© 2024 ポートフォリオサイト | <a href="../contact.html">お問い合わせ</a></p>
    </footer>
</body>
</html>
```

### Markdownテンプレート
```markdown
---
title: "記事のタイトル"
author: "執筆者の名前"
date: "YYYY-MM-DD"
tags: ["技術", "トレンド", "プログラミング"]
description: "この記事では、最新の技術トレンドについて解説します。"
---

# 記事のタイトル

**執筆者:** 執筆者の名前  
**公開日:** YYYY-MM-DD  

## イントロダクション
この記事では、最新の技術トレンドや注目ポイントについて解説します。

## 主題: 最新トレンド
ここで、技術の背景、動向、具体的な事例などを解説します。

- 例: AIの進化とその応用
- 例: Web3の可能性
- 例: サステイナブルな開発手法

## 結論
トピックの要約や、今後の方向性について述べます。
```

