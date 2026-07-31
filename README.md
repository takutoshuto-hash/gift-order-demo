# 首藤卓登 (Takuto Shuto)

食品ギフト企業（社名は非公開）で、EC・Webマーケティングと並行して、**社内の業務システムを内製開発**しています。専門の開発部署がない環境で、現場の困りごとを **自分で動くシステムにして解決する** ことを続けてきました。独学で Google Apps Script や LLM API を使い、外部委託・市販SaaSに頼らず内製化するのが得意です。

- 🛠 要件定義 → 設計 → 実装 → 運用保守までを一人で担当（ソロ開発）
- 🤖 Gemini API・Claude API を実務で活用（OCR／文章生成）
- 💡 「誰がどう使うか」から逆算し、小さく作って価値を出すスタイル

---

## 開発した主なシステム

### 🎁 GiftDesk｜ギフト受注管理システム
申込入力から請求書まで **15機能をブラウザ上のSPAに統合**。1回の入力で、送り状CSV・出荷指示書・熨斗・月次集計・請求書へ自動連携します。FAX注文書は **Gemini API（マルチモーダルLLM）で項目を構造化抽出（JSON）**。
- **技術：** Google Apps Script／スプレッドシート／Gemini API／HTML・CSS・JavaScript（SPA）
- **規模：** 繁忙期は月 1,000〜2,000 件の受注を1人で処理。担当者はスプレッドシートに直接触れない設計。
- 🔗 **ライブデモ（ダミーデータ）：** https://takutoshuto-hash.github.io/gift-order-demo/

### 📍 GBP自社運用システム｜17施設のGoogleビジネスプロフィール運用
グループ17施設の口コミ返信（AI生成＋一括投稿）、検索順位の観測、月次レポート生成を内製化。**API → BigQuery → Looker Studio の監視基盤**を構築し、レポート文面は **Claude API** で自動生成しています。
- **技術：** Google Apps Script／BigQuery／Looker Studio／Claude API／Chrome拡張
- **成果：** 外部委託なら年間約400〜700万円相当の運用を内製で ¥0 化。口コミ返信率100%を維持し、来店行動指標を施策前比 **+66.7%（実測）** に改善。

### 📦 カタログギフト受注管理システム
QR/Web申込受付・ハガキのOCR読み取り・出荷CSV・指示書自動生成・Amazon注文取込を、**一気通貫でデータ化**。
- **技術：** GitHub Pages／Google Apps Script（8ファイル構成）／OCR
- **成果：** 月 100〜200 件の申込を1人で処理。入力ミス率を約5%→0.5%未満に低減。

### 🚚 直送ギフト申込システム（2ブランド）
24時間対応のWeb申込、**銀行CSVによる入金の自動マッチング**、出荷指示書の自動生成、追跡番号の一括メール通知。FAX・手作業中心だった直送業務をWeb・自動化に置き換えました。
- **技術：** Google Apps Script／スプレッドシート／Webフォーム
- **展開：** 同一アーキテクチャを複数ブランドへ横展開。

> ※ 各システムは外部委託・市販SaaSに頼らず内製。運用は原則 Google 無料枠内（¥0）で、顧客データを扱うOCRのみ、学習利用を避けるため有料枠を選択しています。数値は自社の実測・見積りに基づく範囲で記載しています。

---

## 技術スタック

- **言語：** JavaScript（Google Apps Script）／HTML／CSS
- **LLM・AI：** Gemini API／Claude API／Google Cloud Vision API（過去）
- **データ：** Google スプレッドシート／BigQuery／Looker Studio
- **公開・その他：** GitHub Pages／Chrome拡張

---

## これから

独学・ソロで積み上げてきた開発を、**チーム開発の中で正しい設計・技術を身につけながら、より大きな課題に活かしたい**と考えています。特に LLM を実務・事業に落とし込む領域に関心があります。

## リンク

- 🔗 ライブデモ（GiftDesk）：https://takutoshuto-hash.github.io/gift-order-demo/
- 🐙 GitHub：https://github.com/takutoshuto-hash
