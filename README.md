# PortfolioExample_WorX_ENGINEER-CLASS
week9終盤以降で用いる、ポートフォリオ用GitHubの例です

## アプリ概要
例：Next.jsとSupabaseを用いたブログアプリです。  
↑  
面接官が一目で分かるように、使用技術とアプリ概要を端的に記述しましょう。

## サイトイメージ
メインページの画像を貼れると良いです。

![アプリ画面](https://github.com/yusukey354/worx_app/blob/main/docs/dashboard.png?raw=true)

## サイトURL

デプロイした後のアプリのメインページURLを貼りましょう。  
https://operaxis-ooj7i5kyd-yusukey354s-projects.vercel.app/login


「画面中部のゲストログインボタンから、メールアドレスとパスワードを入力せずにログインできます。」といった仕様を作れれば、面接官も試しやすいと思います。

## 使用技術
- フロントエンド：Next.js 15.3
- バックエンド：Next.js 15.3、~Python 3.13.3（FastAPI0.115.12）~
- データベース：Supabase
- デプロイ：Vercel
- バージョン管理：Git、GitHub
- テスト・デバッグ：DevTools（Chrome）
- CI/CD：GitHub Actions（ESLint）

※箇条書きは「-」のあとに空白を入れて本文を始めることで可能です。

## 設計ドキュメント
[要件定義・基本設計・詳細設計の一覧_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/1yBssPgoUI_8TMwVZA2hWOLQj3-l7oirLB2FQ1YJgCww/edit?usp=sharing)

詳細設計時のワイヤーフレーム、ER図、ワークフロー図の画像はdocsディレクトリに格納しています。（[こちらからアクセス](./docs)）

※[]の中に表示文を書き、その後ろで()の中にURLを入れればハイパーリンク化できます。

## 機能一覧
- ユーザー登録、ログイン機能（メールアドレスとパスワード）
- 権限管理
- 指標自動計算
- データ可視化

※空白を2つ開けて「-」から始めることで、箇条書きが2段目になります。三段目は空白を4つ開ければ可能です。

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
