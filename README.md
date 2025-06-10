# operaxis　
KPI可視化ダッシュボードです。

## アプリ概要
Next.jsとSupabaseを用いたKPIの可視化ダッシュボードアプリです。  


## サイトイメージ

![アプリ画面](https://github.com/yusukey354/worx_app/blob/main/docs/dashboard.png?raw=true)

## サイトURL

  
https://operaxis-ooj7i5kyd-yusukey354s-projects.vercel.app/login
テスト用アカウント
test@example.com/password123

「上記アカウントでログインできます。」

## 使用技術
- フロントエンド：Next.js 15.3
- バックエンド：Next.js 15.3、
- データベース：Supabase
- デプロイ：Vercel
- バージョン管理：Git、GitHub
- テスト・デバッグ：DevTools（Chrome）
- CI/CD：GitHub Actions（ESLint）



## 設計ドキュメント
[要件定義・基本設計・詳細設計の一覧_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/1yBssPgoUI_8TMwVZA2hWOLQj3-l7oirLB2FQ1YJgCww/edit?usp=sharing)

詳細設計時のワイヤーフレーム、ER図、ワークフロー図の画像はdocsディレクトリに格納しています。（[こちらからアクセス](./docs)）



## 機能一覧
- ログイン機能（メールアドレスとパスワード）
- 権限管理
- 指標自動計算
- データ可視化



## テスト・修正の設計及び実施書
[テスト・修正の設計及び実施書_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/1ph7XaLu4a2k_kDBEpj_ySTBPETJvg5143ZMk5G90DUA/edit?usp=sharing)

## アプリの改善案
[アプリの改善案_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/15id37P5LLiq2xTsL69gwKxeaVq70L-Wu4XooxUxumRw/edit?gid=1797697990#gid=1797697990)

## 備考
[ESLintの実行結果_GitHub Actions](https://github.com/yusukey354/testapp1/actions/runs/15519197960/job/43690145546)

- 活用した生成AIとその用途
  - ChatGPT：要件定義、設計、各種リサーチ
  - v0：アプリのモック作成
  - GitHub Copilot Chat：ローカル環境でのコードの修正相談

- リファクタリングの規則
  - 2つ以上のファイルで使う、行数が10以上のUIコンポーネントはcomponentsフォルダに移行
  - 2つ以上のファイルで使う、行数が10以上の関数はlibフォルダに移行
  - 変数名で2つ以上の単語が入る場合は、「isPublished」のように二つ目以降の単語の頭を大文字とする
