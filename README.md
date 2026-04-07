# DEJ1 ヘルプ自動計算ツール

Amazon配送パートナー向けヘルプ車割り当て自動計算ツールです。

## 使い方

1. CX（午前）またはMX（午後）を選択
2. アサイン表（.xlsx）をアップロード
3. 「▶ ヘルプ計算を実行」をクリック
4. 結果を確認し「📝 今日の結果を記録する」で保存

## デプロイ手順（初回のみ・約10分）

### 1. GitHubにアップロード

1. https://github.com にアクセスしてサインイン（アカウントがない場合は無料登録）
2. 右上の「+」→「New repository」をクリック
3. Repository name: `dej1-help`
4. Public を選択 → 「Create repository」
5. 「uploading an existing file」をクリック
6. このフォルダの中身（index.html と vercel.json）をドラッグ&ドロップ
7. 「Commit changes」をクリック

### 2. Vercelにデプロイ

1. https://vercel.com にアクセスしてサインイン（GitHubアカウントでログイン可）
2. 「Add New Project」をクリック
3. 先ほど作った「dej1-help」リポジトリを選択
4. そのまま「Deploy」をクリック（設定変更不要）
5. 完了！表示されたURLでアクセス可能になります

### URLの変更（任意）

Vercelのダッシュボード → Settings → Domains から
`dej1-help.vercel.app` などのURLに変更できます。

## 更新方法

index.html を修正して GitHub にアップロードし直すと
Vercel が自動的に最新版を反映します。

## データについて

記録データはブラウザのlocalStorageに保存されます。
同じパソコン・同じブラウザからアクセスした場合のみ履歴が引き継がれます。
複数人で共有する場合は、将来的にバックエンド（データベース）の追加を検討してください。
