# インストールガイド

## Closed Alpha Package

1. GitHub Release `v0.1.0-alpha.1` から assets を取得する。
2. `dist/pbr-channel-audit-docs.zip` を展開して README と manual-test を確認する。
3. repo を clone する場合:

```powershell
git clone https://github.com/Sunmax0731/pbr-channel-audit.git
cd pbr-channel-audit
npm test
```

## Host Setup

1. 作業ディレクトリ `D:\AI\AssetPipeline\pbr-channel-audit` で `npm test` を実行します。
2. `node src/cli/index.js samples/representative-suite.json` を実行し、標準出力の Markdown レポートを確認します。
3. 実素材の JSON に差し替え、失敗と警告の分類を確認します。

