# PBRチャンネル監査

pbr-channel-audit は 3D素材、Unity/Blender向けマテリアルを扱う制作者 向けの closed alpha プロダクトです。BaseColor、Normal、RoughnessなどのPBRチャンネルと命名、欠落を一括監査する。

## Source

- PICKUP Rank: 53
- Domain / Idea No: AssetPipeline / 2
- Repository: pbr-channel-audit
- 主な公開先: GitHub Release / BOOTH
- created_idea: `D:/AI/AssetPipeline/created_idea_002_pbr-channel-audit`
- 同梱ZIP: `D:/AI/AssetPipeline/created_idea_002_pbr-channel-audit/idea_002_pbr-channel-audit.zip`
- 開始時 README: 存在しない


## Alpha Scope

- 代表シナリオ4件の自動検証
- 必須項目不足、警告、混在バッチの分類
- src/cli/ のホスト連携シェル
- QCDS、security/privacy、traceability、release checklist、manual test docs
- docs ZIP: `dist/pbr-channel-audit-docs.zip`

## Commands

```powershell
npm test
node src/cli/index.js samples/representative-suite.json
npm run build:docs
```

手動テストは Codex 側では未実施です。手順は `docs/manual-test.md` と `docs/strict-manual-test-addendum.md` にあります。

