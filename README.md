# lift1up-assets

Lift1up アプリの種目説明ページ用画像アセット (WebP) を GitHub Pages 経由で配信するリポジトリ。

- 配信元: アプリ本体 `alpha-team-inc/torememo`
- 配信URL: https://alpha-team-inc.github.io/lift1up-assets/exercise-pages/{exerciseId}/{asset}.webp
- アップロード: `torememo/scripts/publish-exercise-assets-to-cdn.sh` で同期

アプリ bundle 軽量化 (97% 削減) のため、icon.webp 以外の8素材 (start/finish/step-1〜3/muscle-front/back/advice) をここから取得している。
