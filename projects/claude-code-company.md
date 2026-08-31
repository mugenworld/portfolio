# Claude Company OS — AI-native Operations Experiment

## Overview

**Period:** August 2026 — present  
**Status:** Private internal experiment / active

Claude Company OSは、Claude Codeを単なるコーディングツールではなく、**調査・計画・実装・検証・学習を分担する小さなAI組織として運用できるか**を検証しているプロジェクトです。

目的は「AIを増やすこと」ではなく、AIが速く動くほど必要になる、**役割、権限、確認、記録、検証**をどう設計するかを学ぶことです。

## Problem

複数のAIセッションや複数プロジェクトを使うと、次の問題が起きました。

- 前回の判断が次のセッションへ正しく引き継がれない
- AIごとに同じプロジェクトを違う前提で解釈する
- 「できる操作」と「やってよい操作」が混ざる
- 自動化すると速くなるが、間違いも高速化する
- AI自身の「できました」という報告を、そのまま信用できない

そこで、GitHubを状態と判断の記録場所として使い、人間とAIの責任を明確にする方向へ進みました。

## What Exists Now

private repositoryでは、現在までに主に以下を整備しています。

- Company charter / operating model
- ProjectごとのAI authority
- Architecture Decision Records
- Founder approvalが必要な操作の整理
- Development flow
- Builderとは別コンテキストで成果物を確認するDevelopment Verifier
- 実装前のFact Checkと、実装後のclaim verification
- GitHub Issueを依頼の入口、Pull Requestを結果報告として使うFounder Interface
- 長時間作業時のcheckpoint / stop condition
- 学習素材をnote → adoption → implementationへつなぐAcademy flow
- branch操作などの事故を減らすbest-effort safeguardとregression test
- 外部通信やproduction境界をAIが判断するためのenvironment declaration

## How Work Flows

基本的な流れはシンプルです。

1. Founderが目的を渡す
2. AIが現在のGitHub状態と関連する決定を確認する
3. 作業内容を整理する
4. feature branchで実装する
5. テストする
6. 別コンテキストのVerifierが主張と成果物を確認する
7. Founderへ「何をした / 何が終わった / 何がまだ危険か」を返す
8. mainへの最終反映など重要操作はFounderが判断する

「AIが全部勝手に進める」ことよりも、**安全に任せられる範囲を少しずつ広げる**ことを重視しています。

## Real Use

Company OSはCompany自身を作るためだけの実験ではありません。

実際に別のprivate productであるZOSを対象に、コード監査、E2E runbook作成、通常開発の実装、テスト、Verifierによる確認までを行っています。

この実運用を通して、設計上は正しそうでも実際には不足していた権限境界、停止条件、事実確認、報告形式などを修正してきました。

現在は次の段階として、**外部から受けた小さな仕事も同じCompany flowで処理できるか**を検証しようとしています。

## My Role

私は主に以下を担当しています。

- Companyの目的と原則
- AIに任せる範囲の判断
- 高リスク操作の承認
- 品質基準
- Claude Codeへの依頼
- Claude / Verifierの提案を比較した最終判断
- 実際のProductでCompanyを使い、どこが不足しているかを判断すること

コード、文書、テストの作成にはClaude Codeを大きく利用しています。

## Tools / Concepts

Claude Code / GitHub / Markdown / YAML / shell tests / custom skills / agents / verifier / human-in-the-loop / least-authority thinking

## What I Learned

- Agent数を増やすだけでは組織にはならない
- AIの能力より、操作の可逆性と外部影響で権限を考える方が実用的
- policyを書いただけではtechnical enforcementにはならない
- AIが報告した事実は、可能なら独立に再確認する必要がある
- 自動化する前に、まず手動経路を数回安定して回す方がよい
- Human approvalは自動化の失敗ではなく、意図的なsystem componentになり得る

## Current Direction

現在は、Company OSそのものを完成させることではなく、**ZOS開発や外部案件など本物の仕事をCompanyへ入れ、実戦で必要になった部分だけ改善する**方針です。

長期的には、Founderが目的を話すと、GitHub上の状態を引き継ぎながらAIが実装・検証を進め、Founderは重要判断と成果物確認に集中できる状態を目指しています。

これは現時点で完成した自律会社ではなく、その運用モデルを実測しながら作っている途中のexperimentです。
