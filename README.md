# Eito Kikugawa — AI-assisted Product & Operations Experiments

生成AIを使いながら、個人でプロダクト企画・開発・検証と、AIを使った開発運用の仕組みづくりを続けています。

専門エンジニアとしてすべてのコードを自力で書くことよりも、**課題を整理し、要件を決め、AIに実装させ、結果を検証し、必要なら方向を変えること**を重視しています。

> **Problem → Structure → Build → Verify → Learn → Change**

現在は、次の2つを中心に取り組んでいます。

## Featured Work

### [ZOS — Life Game OS](projects/zos.md)

人生の方向、現実の行動、振り返りをつなぐ「Life Game OS」の実験です。

最初は自己観察ツールとして始まり、Mirror / Persona Mapなどの試作を経て、現在は **Vision / Quest / Mission / Action / Replay / Character** を中心とした構造へ発展しています。

mainにはローカルで動くMVPがあり、後続の実験では会話型オンボーディング、AI Game Master、Vision Map、MCPを使った限定的なデータ連携などを検証しています。

**自分の担当:** 問題設定、コンセプト、要件整理、優先順位、UI/UX判断、AIへの指示、実機検証、採否判断。

---

### [Claude Company OS — AI-native Operations Experiment](projects/claude-code-company.md)

Claude Codeを単なるコーディングツールではなく、**調査・計画・実装・検証・学習を分担する小さなAI組織として運用できるか**を検証している内部実験です。

GitHubを状態の記録場所にし、AIができる操作と人間が決める操作を分け、別コンテキストのAIによる検証、長時間作業の停止条件、Founderへの報告形式などを整備してきました。

現在は、自分のプロダクト開発だけでなく、将来的に外部案件も同じ流れで扱えるかを試す段階に進んでいます。

**自分の担当:** 運用原則、権限境界、品質基準、Founder判断、Claude Codeへの依頼、結果のレビューと採否。

## Earlier Product Experiments

2026年前半には、生成AIを使いながら複数のWebプロダクトを試作しました。

オークション / マーケットプレイス型のフロー、アカウント、入札、決済、管理画面などを含む試作を通して、**MVPの境界、決済を含むE2E検証、機能を増やしすぎる問題、需要検証の重要性**を学びました。

これらは現在の重点プロジェクトではないため、このPortfolioでは個別の詳細ケーススタディとしては掲載していません。

## How I Work with AI

| My responsibility | AI assistance |
|---|---|
| 問題設定・目的の整理 | 調査、比較、選択肢の生成 |
| 要件・優先順位の決定 | 仕様化、実装案の作成 |
| Product / UX判断 | コード生成、修正、レビュー支援 |
| 実機・ブラウザでの確認 | テスト案、矛盾・漏れの検出 |
| 最終的な採否判断 | ドキュメント化、反復作業 |

AIの出力をそのまま正解とは扱いません。可能な範囲で一次情報、実際のコード、テスト結果、GitHub上の状態を確認し、事実と推測を分けて判断することを意識しています。

## Tools / Experience

- ChatGPT / Claude / Claude Code / Codex
- GitHub / Pull Request / branch-based workflow
- AI-assisted research, requirements, implementation and verification
- HTML / CSS / JavaScript
- Next.js / Supabase / Stripeを使った過去の試作経験
- Product discovery / MVP scope / E2E validation

## Current Focus

- AIを使った開発・業務改善を、実案件でも再現できる形にする
- ZOSを自分自身が日常で使えるプロダクトへ近づける
- Claude Company OSを、実際の仕事を安全に処理できる運用へ育てる
- AIが生成した成果物を評価・検証する力を高める

---

This public repository contains written case studies only. Private source code, credentials, customer data, and internal records are not published here.
