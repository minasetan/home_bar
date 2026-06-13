# Home Bar

ホームバーのお酒・材料在庫を JSON で管理し、HTML で閲覧するプロジェクトです。

## ファイル

| ファイル | 説明 |
|---------|------|
| `inventory.json` | 在庫データ（58品目） |
| `schema.json` | JSON Schema |
| `index.html` | 在庫一覧ビューア |

## ローカルで見る

```bash
# Python があれば
python -m http.server 8080
# http://localhost:8080 を開く
```

`file://` では JSON の fetch がブロックされるため、簡易サーバーが必要です。

## GitHub Pages

`main` ブランチの `index.html` がそのまま公開されます。

- リポジトリ: https://github.com/minasetan/home_bar
- サイト: https://minasetan.github.io/home_bar/

## データ形式

各材料は以下のフィールドを持ちます。

- `name` — 在庫名称
- `commonName` — 一般的な名称
- `type` — 種別
- `abv` — 度数（%）
- `description` — 説明
- `group` — カテゴリ
- `addedAt` / `updatedAt` — 追加日・更新日
