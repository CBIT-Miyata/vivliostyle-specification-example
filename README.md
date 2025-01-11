# Vivliostyle 仕様書作成サンプルプロジェクト
このプロジェクトは、Vivliostyleを用いた 仕様書作成のサンプルプロジェクトです。

## 注意事項
- Node.js がインストールされていることが前提です。  
- 推奨バージョン: v18>=

## 使い方

### 環境構築

```bash
$ npm install
```

### プレビューを開始

```bash
$ npm run preview
```

プレビュー中はホットリロードが機能します。

### PDF出力

```bash
$ npm run build
```

## ドキュメントの変更方法
`docs\sample_doc.md` を編集してください。

## スタイルの変更方法
SCSSでのスタイリングを前提としています。  
ルートディレクトリにて、以下を実行してください。

```bash
npm run watch:scss
```

`themes\project-theme\theme.scss` を編集してください。  
`npm run preview` と合わせて使用することで、リアルタイムでスタイルの変更を確認できます。

## 補足

### `<!-- omit in toc -->` について
`<!-- omit in toc -->` は、目次に表示させたくない箇所を指定するためのコメントです。
本プロジェクトでは `Markdown All in One` というVSCodeの拡張機能を使用し、目次を自動生成しています。
目次に表示させたくない箇所がある場合は、このコメントを使用することで目次の自動生成から除外することができます。

## トップページのロゴについて
[こちらのロゴメーカーを使用させていただきました](https://www.shopify.com/jp/tools/logo-maker)