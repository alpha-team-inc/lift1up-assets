# lift1up-assets

Lift1up アプリの種目説明ページ用画像アセット (WebP) を GitHub Pages 経由で配信するリポジトリ。

- 配信元: アプリ本体 `alpha-team-inc/torememo`
- 配信URL: https://alpha-team-inc.github.io/lift1up-assets/exercise-pages/{exerciseId}/{asset}.webp
- アップロード: `torememo/scripts/publish-exercise-assets-to-cdn.sh` で同期

アプリ bundle 軽量化 (97% 削減) のため、icon.webp 以外の8素材 (start/finish/step-1〜3/muscle-front/back/advice) をここから取得している。

## エコシステム内の位置づけ

Lift1up は5プロジェクト構成（torememo / lift1up-app / lift1up-admin / lift1up-lp / lift1up-assets）。本リポジトリは**配信専用**で、画像の正本は torememo `src/assets/exercise-pages/`。**このリポジトリで画像を直接編集せず**、必ず torememo 側のスクリプトから同期する。

- 全体像・連携マップ・データの正マップ: `../lift1up-admin/docs/ecosystem/README.md`（俯瞰ドキュメントの正本）
- ディレクトリ名 `{exerciseId}` は種目マスタの ID と1対1対応し、発行後は変更しない（ID 不変原則）: `../lift1up-admin/docs/ecosystem/source-of-truth.md`
