# CaseMatch — コンテキスト面接 カテゴリーページ

> CaseMatch ビジネスサイト用の「コンテキスト面接とは」カテゴリーページ
> 公開予定: 2026-05-12 / `https://biz.casematch.jp/context-interview/`

## 概要

LLM 時代の AI 面接プラットフォーム CaseMatch が提唱する「コンテキスト面接」のカテゴリー創造ページ。

「従来の AI 面接（カスタムプロパティ型 / Configuration）」と「コンテキスト面接（CaseMatch 型 / Cultivation）」の本質的な違いを、比較表を中心に説明する。

## 構造（Sales Marker `/intent-recruiting/` 準拠）

| セクション | 役割 |
|----------|------|
| Hero（H1）| カテゴリー名直撃で SEO 流入獲得 |
| What | コンテキスト面接の定義 + 三層コンテキスト |
| Why Now | 3 つの構造的変化 |
| 従来との違い（比較表）| **9 軸で Configuration vs Cultivation を可視化** |
| 4 つのポイント | コンテキスト面接の構成要素 |
| 事例 | INTLOOP 系 / シグマクシス系 |
| CaseMatch とは + 3 つの差別化 | プロダクト訴求 |
| FAQ | 想定質問への統一回答 |
| CTA | 30 分個別デモへの導線 |

## ローカルプレビュー

```bash
# Mac
open index.html

# or simple HTTP server
python3 -m http.server 8000
# → http://localhost:8000/
```

## デプロイ想定

### Option A: GitHub Pages
```bash
# このリポを GitHub にプッシュ後
# Settings → Pages → main branch / root を選択
# https://[username].github.io/casematch-context-interview/ で公開
```

### Option B: 既存サイトへの統合
- biz.casematch.jp の `/context-interview/` ディレクトリに配置
- 既存 Next.js / WordPress 等のフレームワークに合わせて移植

## 技術スタック

- **HTML5** 単独ファイル（メンテ性重視）
- **Tailwind CSS** CDN 経由（ビルド不要）
- **レスポンシブ対応**（モバイル / タブレット / デスクトップ）
- **アクセシビリティ**: セマンティック HTML / `<details>` で FAQ アコーディオン

## SEO 設計

| 項目 | 内容 |
|------|------|
| Title | コンテキスト面接とは｜CaseMatch — LLM時代のAI面接プラットフォーム |
| Description | 120字以内・KW直撃 |
| OGP | OG title / description / type |
| 構造化データ | （将来追加）Article / FAQPage / BreadcrumbList |

## メイン KW

| 優先 | KW |
|------|-----|
| ★★★ | コンテキスト面接 |
| ★★★ | コンテキスト面接 とは |
| ★★ | AI 面接 中途採用 |
| ★★ | AI 面接 カスタマイズ |
| ★ | ジョブ型 採用 |

## 設計方針メモ

- **Configuration vs Cultivation の対比** が比較表のコア概念
- 「他社は『設定する』、CaseMatch は『育てる』」のキーフレーズを Hero、比較表、CTA で繰り返し表示
- 競合（PreferredAI / VARIETAS / PeopleX / マイナビ×MQ）への直接言及はせず、4 類型マップで間接的にポジショニング
- 中途専門職ターゲットの強調（「ハイクラス採用」「ジョブ型」キーワード）

## 関連ドキュメント

- `category-page-context-interview-v1.md`（仕様 SoT）
- `context-interview-guideline-v1.md`（社内アライメント）
- `battlecard-3competitors-v1.md`（競合バトルカード）

---

更新履歴:
- v1（2026-04-30）: 初版実装
