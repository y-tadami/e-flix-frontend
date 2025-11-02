# E-FLIX Frontend

E-FLIXは、社内向けの講義動画プラットフォームです。  
このリポジトリはフロントエンド（React + Vite）プロジェクトです。

## 主な機能

- Googleアカウント（@estyle-inc.jp）による認証
- 講義動画の一覧・検索・カテゴリ表示
- マイリスト・視聴履歴管理
- Firebaseによるデータ管理
- FlaskバックエンドAPIとの連携

## セットアップ手順

1. リポジトリをクローン

    ```bash
    git clone <このリポジトリのURL>
    cd e-flix-frontend
    ```

2. 依存パッケージのインストール

    ```bash
    npm install
    ```

3. `.env` ファイルを作成し、必要な環境変数を設定  
   （例: FirebaseのAPIキーやAPIエンドポイント）

4. 開発サーバーの起動

    ```bash
    npm run dev
    ```

## 環境変数（.env例）

```env
VITE_FIREBASE_API_KEY="..."
VITE_FIREBASE_AUTH_DOMAIN="..."
VITE_FIREBASE_PROJECT_ID="..."
VITE_FIREBASE_STORAGE_BUCKET="..."
VITE_FIREBASE_MESSAGING_SENDER_ID="..."
VITE_FIREBASE_APP_ID="..."
VITE_ALLOWED_DOMAIN="@estyle-inc.jp"
VITE_API_URL="http://127.0.0.1:5000/api/videos"
```

## その他

- 本番環境用には`.env.production`を利用してください。
- `.env`ファイルはGit管理対象外です。

---

## ライセンス

社内利用限定
