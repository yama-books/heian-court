# CHECKPOINT｜平安貴族ゲーム・設計基盤 F0

- 記録日: **2026-11-04 JST**
- 開発正本: https://github.com/yama-books/heian-court （Public）
- 作成元: https://github.com/moyashimisosoup/app-factory/issues/18
- Repo作成Actions: https://github.com/moyashimisosoup/app-factory/actions/runs/41666014046 （SUCCESS）
- 基盤設計統合PR: https://github.com/yama-books/heian-court/pull/1
- PR #1統合時のmain HEAD: `d8d01d778c516cc81f141589b84bb4e54d6d51c9`

## 目的
構想を実装から分離し、史実に基づく宮廷人生ゲームのために、開発担当者が参照できる設計基盤をつくる。

## 保存・検証済み
- `README.md`、`AGENTS.md`、`docs/PRODUCT_VISION.md`、`docs/GAME_DESIGN.md`、`docs/HISTORICAL_RESEARCH.md`、`docs/ASYNC_SOCIAL.md`、`docs/DECISIONS.md`、`docs/ROADMAP.md` の8ファイルをPR #1経由でmainに統合。
- 8ファイルすべてをmainから読戻し、内容とリンク構成を確認。
- 最初の題材は一条朝・西暦1000年前後。A（一人用人生シミュレーション）＋B（自律NPC箱庭）、来歴閲覧、定型文の手紙、匿名集計の遅延反映を基本方針とする。
- 位階と官職、形式的権威と実権、史実・解釈・信仰・文学・ゲーム創作を区別する規則を記録。

## 未実施と注意点
- 人物30〜50名の一次・二次史料による検証、官職・任官・家系・年次の確定は未実施。文書の「出典候補」は出発点であり、精査済みデータセットではない。
- 出自選択・ゲームループ・NPC・列伝を動かすWebアプリは未実装。CI、GitHub Pages、API、オンライン共有、PC/スマホでの実機確認も未実施。
- APP-IDは正式未採番。Session Deck台帳の最新掲載IDと、別途進行している複数アプリの採番に差があるため、重複を解消した後に登録する。
- このCHECKPOINTも設計保存の証拠であり、ユーザーによるゲーム性の検収を意味しない。

## 次の一操作
`docs/HISTORICAL_RESEARCH.md`を基準に、一条朝の**西暦1000年前後の人物30〜50名の候補表**（出典・年次・官職・家系・同時代性・未確認フラグ）を作成する。実装を急がず、最初に「史実として確定できるもの」と「ゲーム用創作」の境界を検証する。

## 引継ぎ
- スコープ: 歴史調査・ゲーム設計。ユーザーの次の明示依頼がない限りPages公開や本体実装を行わない。
- ブランチ/HEAD: 上記PR #1のmain HEADを検証基点とし、**作業開始時に最新main/PR/CIを再照合**すること。
- 参照先: [README](../../README.md)、[ROADMAP](../ROADMAP.md)、[DECISIONS](../DECISIONS.md)、[HISTORICAL_RESEARCH](../HISTORICAL_RESEARCH.md)。
