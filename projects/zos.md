# ZOS — Life Game OS

## Overview

**Period:** May 2026 — present  
**Status:** Private product / active experiment

ZOSは、人生の方向、現実の行動、振り返りを一つの流れとして扱う「Life Game OS」の実験です。

最初は自己観察を助けるツールとして始まりましたが、試作を続ける中で「自分を理解するだけでは現実の行動に戻れない」という課題が見え、現在は **Vision / Quest / Mission / Action / Replay / Character** を中心とした構造へ発展しています。

## Product Evolution

これまでに、主に次の方向を試してきました。

- **Mirror** — 反応、感情、未解決の問いを記録する
- **Persona Map** — 自分の役割や信念などを視覚的に整理する
- **Action / Replay** — 現実で行動し、その結果を振り返る
- **Life Game model** — Visionから日々のActionまでをゲームの構造として扱う
- **Vision Map** — QuestやMission、分岐、方向転換を一枚の地図として扱う
- **AI Game Master experiments** — 会話から現在地や次の一手を整理する

## Current MVP

private repositoryのmainには、ローカルで動くMVPがあります。

主な要素:

- 日本語オンボーディング
- Vision / Quest / Action
- Actionの開始・完了・中断・見送り
- Replay
- Character observation
- local data persistence / reload recovery
- Save Data export / import
- Mirror / Persona Mapの既存資産

現時点では「完成したプロダクト」としてではなく、実際に使いながら世界観・データ構造・行動ループを検証するためのMVPとして扱っています。

## Later Experiments

mainとは別の実験では、以下を検証しています。

- 会話型の初期設定
- AI Game Master
- Vision Mapのgraph model
- AIの提案と本人確認を分けるController
- MCPを使った限定的なread / proposal / confirmed write
- local-firstなSave DataとAI providerの分離

これらはすべて一つの完成版として公開済みという意味ではなく、次の製品世代に向けた検証です。

## My Role

私は主に以下を担当しています。

- 問題設定とコンセプト
- 要件整理とMVP範囲
- UI / UXと言葉の判断
- 何を作るか・作らないかの決定
- Claude Code / CodexなどAIへの指示
- ブラウザ・実機での動作確認
- AIが作った実装の採否
- 仕様変更と優先順位の判断

コード実装には生成AIを大きく利用しています。すべてのコードを自力で書いたという説明はしていません。

## Tools / Concepts

HTML / CSS / JavaScript / localStorage / PWA / GitHub / Claude / Claude Code / Codex / MCP experiments

## What I Learned

- 実際に触れる試作品を作ることで、最初の問題設定そのものが変わることがある
- AIは矛盾した要求でも高速に実装できるため、境界と正本が重要
- 機能数より「現実へ戻れる一つのループ」の方が価値を検証しやすい
- AIは本人の人生を決定するauthorityではなく、提案と観察を支援する存在として扱う必要がある
- 保存、復元、移行、権限もProduct Experienceの一部

## Current Direction

現在の焦点は、機能を増やすこと自体ではなく、**AIとの会話や現実で起きた変化がQuest / Mission / Action / Replayとして整理され、自分が日常的に使いたくなる体験になるか**を検証することです。
