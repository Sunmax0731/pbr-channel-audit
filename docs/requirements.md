# 要件定義

## 目的

PBRチャンネル監査 は、3D素材、Unity/Blender向けマテリアルを扱う制作者 が BaseColor、Normal、RoughnessなどのPBRチャンネルと命名、欠落を一括監査する。

## Source

- PICKUP Rank: 53
- Domain / Idea No: AssetPipeline / 2
- Repository: pbr-channel-audit
- created_idea: `D:/AI/AssetPipeline/created_idea_002_pbr-channel-audit`
- ZIP: `D:/AI/AssetPipeline/created_idea_002_pbr-channel-audit/idea_002_pbr-channel-audit.zip`
- README確認: 開始時点では正式 repo が存在しないため、README.md は存在しない。

## Functional Requirements

- R1: materialName、requiredChannel、texturePath、colorSpace を必須項目として検査する。
- R2: 必須項目不足は fail として分類する。
- R3: `colorSpaceRisk` が true の場合は warning として分類し、手動確認理由を返す。
- R4: 複数アイテムの mixed-batch を pass / warning / fail に集計する。
- R5: 結果を CLI と docs/release evidence で再利用できる形にする。

## Non Functional Requirements

- UTF-8 で Markdown / JSON / JS / HTML / Python を保存する。
- 外部通信を既定で行わず、サンプルとローカル入力だけで検証できる。
- 手動テスト未実施であることを release 前 docs に明記する。

