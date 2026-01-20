# 受発注管理システム - 株式会社食彩厨房やくも

居酒屋・日本酒バー・ビアバー向けの受発注管理システム

## 🏢 会社情報

- **会社名**: 株式会社食彩厨房やくも
- **業種**: 居酒屋、日本酒バー、ビアバー
- **住所**: 北海道札幌市中央区大通東2-3-1 第36桂和ビル B2F
- **電話番号**: 050-5600-7609
- **従業員数**: 7人
- **HP**: https://tabelog.com/hokkaido/A0101/A010102/1051825/

## 🔐 ログイン情報

- **ユーザー名**: `食彩厨房やくも`
- **パスワード**: `admin123`

## 📦 主な仕入先

1. **北海道鮮魚卸** - 鮮魚（マグロ、サーモン、ホタテ、イカ、ホッケ、カニ、ウニ）
2. **札幌酒類販売** - 酒類（日本酒、焼酎、ビール）
3. **道産野菜センター** - 青果（じゃがいも、玉ねぎ、アスパラガス、大根）
4. **北の食肉センター** - 食肉（ラム肉、豚肉、鶏肉、牛タン）

## 📊 機能

- ✅ ダッシュボード（売上・費用・利益の可視化）
- ✅ 顧客管理
- ✅ 伝票管理（見積書・納品書・請求書）
- ✅ 仕入先管理（銀行情報含む）
- ✅ 発注管理
- ✅ 会計管理（仕訳・試算表・損益計算書・貸借対照表）
- ✅ CSVエクスポート

## 🚀 デプロイ

### Vercelへのワンクリックデプロイ

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fkazunarihonda83-jpg%2Forder-management-system-yakumo&env=NODE_ENV,JWT_SECRET,VERCEL&envDescription=Required%20environment%20variables%20for%20deployment&envLink=https%3A%2F%2Fgithub.com%2Fkazunarihonda83-jpg%2Forder-management-system-yakumo%2Fblob%2Fmaster%2FVERCEL_%25E3%2583%2587%25E3%2583%2597%25E3%2583%25AD%25E3%2582%25A4_%25E7%25B0%25A1%25E5%258D%2598%25E6%2589%258B%25E9%25A0%2586.md)

または、手動でデプロイ：

### 手動デプロイ手順

1. **https://vercel.com/new** にアクセス
2. GitHubアカウントでログイン
3. **order-management-system-yakumo** リポジトリをインポート
4. 環境変数を設定：
   - `NODE_ENV=production`
   - `JWT_SECRET=yakumo-secret-key-2025-production-secure`
   - `VERCEL=1`
5. **Deploy** をクリック

詳細な手順は [VERCEL_デプロイ_簡単手順.md](./VERCEL_デプロイ_簡単手順.md) を参照してください。

## 💻 開発環境

### ローカル起動

```bash
# 依存関係のインストール
npm install

# フロントエンド開発サーバー起動
npm run dev

# バックエンドサーバー起動
npm run server
```

### ビルド

```bash
npm run build
```

## 🛠️ 技術スタック

- **フロントエンド**: React 18.3 + Vite
- **バックエンド**: Node.js + Express.js
- **データベース**: SQLite3
- **認証**: JWT
- **デプロイ**: Vercel Serverless Functions

## 📝 サンプルデータ

初回起動時に以下のサンプルデータが自動的に作成されます：

- 管理者ユーザー: 食彩厨房やくも
- 仕入先: 4社（鮮魚、酒類、青果、食肉）
- 発注データ: 5件（本マグロ、日本酒、野菜、ラム肉など）

## ⚠️ 注意事項

### データベースについて

Vercel環境では、SQLiteを`/tmp`ディレクトリに保存しています。
`/tmp`のデータは永続化されないため、本番運用では以下を推奨：

- **Vercel Postgres** (推奨)
- **Supabase**
- **PlanetScale**
- **Neon**

### セキュリティ

- `JWT_SECRET`は必ず強力なランダム文字列に変更してください
- 本番環境では管理者パスワードを変更してください

## 📞 サポート

システムに関するお問い合わせは、開発元までご連絡ください。

---

**作成日**: 2025-01-20  
**バージョン**: 1.0.0  
**対応会社**: 株式会社食彩厨房やくも
