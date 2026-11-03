# 平安貴族ゲーム（heian-court）

**状態：調査・設計／ゲーム未実装／GitHub Pages未公開**

平安朝の官職・家系・婚姻・宮廷人脈を学びながら、さまざまな出自から一生を生きるWebゲームの構想。

正式な強さランキングではなく、**人物ごとの来歴**を残し、他のプレイヤーの人生を閲覧する。自分の宮廷では自律NPCが動き、他の参加者の行動傾向が「宮中の風聞」としてゆるやかに反映されることを目指す。

## 設計の入口

| ファイル | 内容 |
| --- | --- |
| [PRODUCT_VISION](docs/PRODUCT_VISION.md) | 目的・体験の核・やらないこと |
| [GAME_DESIGN](docs/GAME_DESIGN.md) | 出自選択、役職、人物関係、人生シミュレーション |
| [HISTORICAL_RESEARCH](docs/HISTORICAL_RESEARCH.md) | 史実・文学・信仰・創作の区別、調査出典、データ採用条件 |
| [ASYNC_SOCIAL](docs/ASYNC_SOCIAL.md) | 列伝共有、定型文の消息、遅延集計と安全性 |
| [DECISIONS](docs/DECISIONS.md) | 決まったことと未確定事項の境界 |
| [ROADMAP](docs/ROADMAP.md) | 小さな試作に向けた段階計画 |
| [AGENTS.md](AGENTS.md) | 開発・検証・記録上の共通規則 |

## 重要な方針

- **A＋B方式**：一人用の人生選択＋自律NPCの宮廷箱庭。オンライン同期をゲーム成立の前提にしない。
- **初期時代**：一条朝の西暦1000年前後を優先して調査。摂関政治と後期院政は混在させない。
- **公的地位と実権を分離**：位階・官職・婚姻・人脈・後見・財力の関係から選択肢を作る。
- **出自は固定も抽選も可能にする構想**：「運命に任せる」「生き方から選ぶ」「立場を指定」を検討。
- **非同期交流は後続工程**：公開に同意した人物列伝、審査済み定型文の消息、匿名集計の宮廷情勢。自由チャットは禁止。
- **史実の正確性**：史実、解釈、当時の信仰、文学、ゲーム創作を別データとする。

## 現在の到達点と次の一操作

App Factory [Issue #18](https://github.com/moyashimisosoup/app-factory/issues/18)から、[作成Run #41666014046](https://github.com/moyashimisosoup/app-factory/actions/runs/41666014046)で `yama-books/heian-court` を**Public**に作成済み。初期main commit: `e755fb6cb59508dc0ed0b3c6c5bfed4bb495c0c1`。

設計基礎文書をGitHubに配置する段階。**現状はゲーム本体コード・ブラウザ試作・API・Pages公開・実機テストのいずれも未実施**。

次は、史実採用のための「一条朝1000年前後の人物・官職・婚姻・後見・年次」を出典付き候補表として整理する。最初から全機能を実装せず、小さな試作へつなげる。

> APP-IDはSession Deck台帳との採番整合を確認してから正式確定する。
