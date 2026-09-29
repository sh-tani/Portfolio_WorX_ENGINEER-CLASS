# Portfolio_WorX_ENGINEER-CLASS

## アプリ概要
Next.jsとSupabaseを用いた登山の予定管理・計画補助アプリです。

## サイトイメージ

![アプリ画面](https://github.com/sh-tani/Portfolio_WorX_ENGINEER-CLASS/blob/d6de238b919acbe7f6bc0bb7d2917c0684ca61f6/docs/%E3%82%A2%E3%83%97%E3%83%AA%E3%81%AE%E3%83%A1%E3%82%A4%E3%83%B3%E3%83%9A%E3%83%BC%E3%82%B8%E7%94%BB%E5%83%8F.png?raw=true)

## サイトURL

https://yamatabi-planner.vercel.app/
「一部の機能はログインせずにゲストモードとして試すことができます。」

## 使用技術
- フロントエンド：Next.js 16.3.3
- バックエンド：Next.js 16.3.3
- データベース：Supabase
- デプロイ：Vercel
- バージョン管理：Git、GitHub
- テスト・デバッグ：DevTools（Chrome）
- CI/CD：GitHub Actions（ESLint）


## 設計ドキュメント
[要件定義・基本設計・詳細設計の一覧_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/1DZGjB_i8kyIdmLThLy9QimfQoCkisRKI95MAbz4pGZ0/edit?gid=0#gid=0)

詳細設計時のワイヤーフレーム、ER図、ワークフロー図の画像はdocsディレクトリに格納しています。（[こちらからアクセス](./docs)）

## 機能一覧
- ユーザー登録、ログイン機能（メールアドレスとGoogleアカウント）
- 予定登録機能
- 予報に応じたおすすめ度の算出機能

## テスト・修正の設計及び実施書
[テスト・修正の設計及び実施書_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/19bm9xpost1KeBzw9kJJPMmsAUKpjzRaUpupmFMVmeOU/edit?usp=sharing)

## アプリの改善案
[アプリの改善案_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/1ucYvypE9kCnSirvhEIeS9SnbHmBWuXX1j5jyS2leMlA/edit?usp=sharing)

## 備考
[ESLintの実行結果_GitHub Actions](https://github.com/sh-tani/holiday-planner/actions)

- 活用した生成AIとその用途
  - ChatGPT：要件定義、設計、各種リサーチ
  - v0：アプリのモック作成
  - GitHub Copilot Chat：ローカル環境でのコードの修正相談

- リファクタリングの規則
  - 2つ以上のファイルで使う、行数が10以上のUIコンポーネントはcomponentsフォルダに移行
  - 2つ以上のファイルで使う、行数が10以上の関数はlibフォルダに移行
  - 変数名で2つ以上の単語が入る場合は、「isPublished」のように二つ目以降の単語の頭を大文字とする
