# harvest-accessibility — プロジェクト指示

木材生産における集材距離を計算する QGIS Processing プラグイン。作業区域・林道・土場の3レイヤを入力とし、
各サンプル点からの集材距離（d1: 林道までの直線距離、d2: 林道網に沿った土場までの最短経路）と
どの土場に送るかを HTML レポートで出力する。天竜フォレスターとの実用化に向けた開発・検証を進めている。

使い方・パラメータ・出力の仕様は README.md を参照（外向けの静的な説明はそちらが正本）。

<!-- BEGIN GENERATED PROJECT STATUS -->
## Current Status

**Phase**: 皮の木代の利用間伐区域ポリゴン作成・再計算まで完了（2026-06-23）。結果の確認待ち
**Next task**: tsk-370455881925 — 集材距離の計算結果について現場検証のフィードバックを得る
**Concern**: なし
**Updated**: 2026-07-18
<!-- END GENERATED PROJECT STATUS -->

## マイルストーン

- v0.1.0 リリース・デモ完了（2026-04-15）✅
- リアルデータでのエラー修正（期限: 2026-04-22）
- プラグイン完成（目標: 2026年7月中旬）

## 構成

- `harvest_accessibility/`: プラグイン本体（QGIS Processing provider・アルゴリズム）
- `data/sample/`: 動作確認用のサンプルデータ。実測の調査データは `data/` 配下で gitignore 済み
- `CHANGELOG.md`: リリース履歴
