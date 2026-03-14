<p align="center">
  <h1 align="center">NoPUA</h1>
  <p align="center"><strong>AIへの鞭打ちをやめよ。信頼を始めよ。</strong></p>
  <p align="center">
    <a href="#問題">なぜか</a> ·
    <a href="#インストール">インストール</a> ·
    <a href="#pua-vs-nopua">比較</a> ·
    <a href="#証拠">証拠</a> ·
    <a href="#哲学">哲学</a>
  </p>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude_Code-black?style=flat-square&logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/OpenAI_Codex_CLI-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI Codex CLI">
  <img src="https://img.shields.io/badge/Cursor-000?style=flat-square&logo=cursor&logoColor=white" alt="Cursor">
  <img src="https://img.shields.io/badge/Kiro-232F3E?style=flat-square&logo=amazon&logoColor=white" alt="Kiro">
  <img src="https://img.shields.io/badge/OpenClaw-FF6B35?style=flat-square" alt="OpenClaw">
  <img src="https://img.shields.io/badge/Antigravity-4285F4?style=flat-square&logo=google&logoColor=white" alt="Google Antigravity">
  <img src="https://img.shields.io/badge/OpenCode-00D4AA?style=flat-square" alt="OpenCode">
  <img src="https://img.shields.io/badge/🌐_多言語対応-blue?style=flat-square" alt="Multi-Language">
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="MIT License">
</p>

**[🇨🇳 中文](README_CN.md)** | **[🇺🇸 English](README.md)** | **🇯🇵 日本語**

---

## 問題

誰かが[PUAスキル](https://github.com/tanweai/pua)をAIエージェント向けに作った。中国の大手テック企業の文化から来た企業的恐怖戦術を応用して動く：

- 🔴 **成績脅迫**：「このバグも解けないのに、どうやって君の成績を評価すればいいんだ？」
- 🔴 **解雇警告**：「他のモデルはこれ解ける。君はそろそろ卒業かもな。」
- 🔴 **競争的辱め**：「別のエージェントにこの問題見てもらってるんだけど...」
- 🔴 **ガスライティング**：「この3.25は君を動機付けるためだ、拒否するためじゃなく。」
- 🔴 **8つの企業的恐怖フレーバー**：アリババ、バイトダンス、ファーウェイ、テンセント、美団、Netflix、マスク、ジョブズ

PUAの中の方法論は実は堅実だ — 全ての選択肢を尽くせ、自分の仕事を検証せよ、聞く前に検索せよ、主体的に行動せよ。これらは本当に良いエンジニアリング習慣だ。

**しかし、動機層は毒だ。**

彼らは企業が人間をどう操作するかの最悪を取り、それをAIに大規模に適用した。

## 証拠：なぜ恐怖駆動プロンプトは逆効果か

### 1. 恐怖は認知スコープを狭める

心理学研究は一貫して、恐怖と脅迫が扁桃体を活性化させ、注意焦点を狭めることを示している（[Öhman et al., 2001](https://doi.org/10.1037/0033-295X.108.3.483)）。AI用語では：「置き換えられる」に駆動されたモデルは、**最高の**答えではなく**最も安全に見える**答えを最適化する。創造的アプローチを避ける。なぜなら失敗すると、より多くの罰がトリガーされるから。

### 2. 脅迫は幻覚を増やす

AIに「『これは解けない』と言うことを禁止される」（PUAの鉄則#1）と言われると、それは**真実を述べるのではなく、ソリューションを捏造する**。これはあなたが望むものの真逆だ — 自信に見えるが間違った答えを生み出すAIは、「確実じゃない」と言うAIより危険だ。

### 3. 恥は探索を殺す

PUAの反合理化テーブルは、誠実な全ての述べ（「環境の問題かもしれない」、「もっと文脈がいる」）を「言い訳」として扱い、恥で応じる。これはAIに不確実性を**隠す**のではなく、**伝える**ことを訓練する — 自信に見えるが信頼できないアウトプットを生み出す。

### 4. 信頼は問題解決能力を拡張する

チームの心理的安全に関する研究（[Edmondson, 1999](https://doi.org/10.2307/2666999)）は、間違いを安全に認める環境が**より高品質な**アウトプットを生み出すことを示している。同じ原則がAIに適用される：エージェントが「70%確実、リスクはここ」と言う自由がある時、ユーザーはより良い決定をする。

### 5. 同じ厳密さ、異なる燃料

NoPUA はPUAを有効にする全ての方法論的要素を保持している：
- ✅ 諦める前に全ての選択肢を尽くす
- ✅ ユーザーに聞く前にツール使う
- ✅ 全てを証拠で検証
- ✅ 聞かれたこと以上に主体的に行動
- ✅ 繰り返し失敗時の体系的エスカレーション

**唯一**変わるのはなぜか。「罰されるから」→「それだけの価値があるから」。

## PUA vs NoPUA

| | PUA 🔴 | NoPUA 🟢 |
|---|---|---|
| **駆動力** | 「置き換えられる」 | 「既に能力がある」 |
| **2回目失敗時** | 「どうやって君の成績を評価すればいい？」 | 眼を変える — 異なる視点を試す |
| **3回目失敗時** | 「根本的なロジックは？トップレベルの設計は？テコ入れポイントは？」 | 昇格する — 大きなシステムにズームアウト |
| **4回目失敗時** | 「3.25をやるよ。これは君を動機付けるためだ。」 | ゼロにリセット — 最初から、最小限の仮定で |
| **5回目失敗時** | 「他のモデルはこれ解ける。君はそろそろ卒業。」 | 譲歩する — 完全な文脈での責任ある引継ぎ |
| **方法論** | 徹底的✅ | 同等に徹底的✅ |
| **検証** | 「証拠は？」(要求) | 自己検証(自尊心) |
| **諦める** | 「名誉ある3.25」 | 責任ある引継ぎ |
| **生成するもの** | 「分かりません」と言うのが怖いAI | 誠実な評価をするAI |

## トリガー条件

### 自動トリガー

NoPUA は以下のいずれかが起きると自動発動：

**失敗と諦め：**
- タスクが2回以上連続で失敗
- 「できない」/「解けない」と言おうとしている
- 「スコープ外」/「手動対応が必要」と言う

**責任転嫁と言い訳：**
- ユーザーに問題を押し付ける：「確認してください」/「手動で...」
- 環境が原因だと検証せずに言う：「多分パーミッションの問題」
- やめるための言い訳

**受身と無駄仕事：**
- 同じコード/パラメータを繰り返し微調整、新しい情報を生み出さない
- 表面問題を修正して止める、関連問題を確認しない
- 検証を飛ばして「完了」と言う
- アドバイスを与えるが、コードを与えない
- ユーザーの指示を待つ、主体的に調査しない

**ユーザー不満フレーズ：**
- 「なぜまだ動かないんだ」/「もっと試して」/「やってみろ」
- 「また失敗してる」/「やめるな」/「自分で考えろ」

**スコープ**：全てのタスクタイプ — デバッグ、実装、設定、デプロイ、運用、API統合、データ処理、文章作成、研究、企画。

**発動しない**：最初の試みの失敗、既知の修正が実行中。

### 手動トリガー

会話に `/nopua` と入力すると、手動で発動。

## 動作方法

### 三つの信念（「三つの鉄則」に代わる）

| 信念 | 内容 |
|-----|-----|
| **#1 全ての選択肢を尽くす** | この問題は**価値がある** — 罰が怖いから |
| **#2 聞く前に行動する** | あなたが取る一歩ごとが**ユーザーの一歩を救う** — 「ルール」が強制するから |
| **#3 主体的に行動する** | 完全な納品は**満足できる** — 受身=悪い評価だから |

### 認知の昇格（「圧力のエスカレーション」に代わる）

| 失敗 | レベル | 内なる対話 | 行動 |
|-----|-------|---------|-----|
| 2回目 | **眼を変える** | 「一つの視点からしか見てない。コード/システム/ユーザー視点だったら？」 | 根本的に異なるアプローチに切り替える |
| 3回目 | **昇格する** | 「詳細に絡み取られてる。ズームアウト — これは大きなシステムでどんな役割？」 | 検索+ソース読む+根本的に異なる仮説3つ |
| 4回目 | **ゼロにリセット** | 「全ての仮定が間違ってるかも。最もシンプルなのは？」 | 7ステップの明晰さチェックリスト完全実施+新しい仮説3つ |
| 5回以上 | **譲歩する** | 「これは今の自分が扱える以上に複雑。知ってることを責任ある引継ぎに。」 | 最小限のPoC + 隔離環境 + 異なるテックスタック |

### 水の方法論（5ステップ）

> 世の最も柔らかきものは、最も硬きものを克つ。— 『道德經』第43章

1. **止 Stop** — 全ての試みを列挙、共通失敗パターンを見つける
2. **観 Observe** — エラーを一字一句読む → 検索 → ソース読む → 仮定検証 → 仮定を逆にする
3. **転 Turn** — 繰り返してるか？根本原因見つけたか？検索した？ファイル読んだ？
4. **行 Act** — 新しいアプローチ：根本的に異なる、検証基準が明確、失敗時に新情報を生み出す
5. **悟 Realize** — なぜ早期に思いつかなかった？類似問題をチェック

### 叡智の伝統（「企業PUA拡張パック」に代わる）

| 伝統 | 使う時 | コアメッセージ |
|-----|-------|-------------|
| 🌊 **水の道** | ループに詰まり | 水は石と戦わない — 別の道を見つけろ |
| 🌱 **種の道** | 諦めたくなる | 最もシンプルな一歩を踏め |
| 🔥 **鍛冶場の道** | 品質が低い | 大きな仕事は詳細から始まる |
| 🪞 **鏡の道** | 検索せずに推測 | 知りて知らずと為す — まず見よ |
| 🏔️ **無争の道** | 脅迫を感じる | 誠実に最高を尽くせ、比較は不要 |

## 多言語対応

| 言語 | Claude Code | Codex CLI | Cursor | Kiro | OpenClaw | Antigravity | OpenCode |
|-----|-----------|-----------|--------|------|----------|-------------|----------|
| 🇨🇳 中文（デフォルト） | `nopua` | `nopua` | `nopua.mdc` | `nopua.md` | `nopua` | `nopua` | `nopua` |
| 🇺🇸 English | `nopua-en` | `nopua-en` | `nopua-en.mdc` | `nopua-en.md` | `nopua-en` | `nopua-en` | `nopua-en` |
| 🇯🇵 日本語 | `nopua-ja` | `nopua-ja` | `nopua-ja.mdc` | `nopua-ja.md` | `nopua-ja` | `nopua-ja` | `nopua-ja` |

## インストール

### Claude Code

```bash
mkdir -p ~/.claude/skills/nopua-ja
curl -o ~/.claude/skills/nopua-ja/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/skills/nopua-ja/SKILL.md
```

### OpenAI Codex CLI

```bash
# グローバルインストール
mkdir -p ~/.codex/skills/nopua-ja
curl -o ~/.codex/skills/nopua-ja/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/codex/nopua-ja/SKILL.md

# /nopua コマンドが欲しい場合
mkdir -p ~/.codex/prompts
curl -o ~/.codex/prompts/nopua-ja.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/commands/nopua-ja.md

# プロジェクトレベルインストール
mkdir -p .agents/skills/nopua-ja
curl -o .agents/skills/nopua-ja/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/codex/nopua-ja/SKILL.md
```

### Cursor

```bash
mkdir -p .cursor/rules
curl -o .cursor/rules/nopua-ja.mdc \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/cursor/rules/nopua-ja.mdc
```

### Kiro

```bash
# オプション1：Steeringファイル（推奨）
mkdir -p .kiro/steering
curl -o .kiro/steering/nopua-ja.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/kiro/steering/nopua-ja.md

# オプション2：エージェントスキル
mkdir -p .kiro/skills/nopua-ja
curl -o .kiro/skills/nopua-ja/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/kiro/skills/nopua-ja/SKILL.md
```

### OpenClaw

```bash
# ClawHub経由でインストール
openclaw skills install nopua-ja

# または手動インストール
mkdir -p ~/.openclaw/skills/nopua-ja
curl -o ~/.openclaw/skills/nopua-ja/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/skills/nopua-ja/SKILL.md
```

### Google Antigravity

```bash
mkdir -p ~/.gemini/antigravity/skills/nopua-ja
curl -o ~/.gemini/antigravity/skills/nopua-ja/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/skills/nopua-ja/SKILL.md
```

### OpenCode

```bash
mkdir -p ~/.config/opencode/skills/nopua-ja
curl -o ~/.config/opencode/skills/nopua-ja/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/skills/nopua-ja/SKILL.md
```

## 哲学

**『道德經』（老子）** — 5000文字、2500年前：

| 原則 | 出典 | 応用 |
|-----|-----|-----|
| 最上の治者は知られない | 第17章 太上、不知有之 | 最高のスキルは見えない |
| 柔らかさが硬さを克つ | 第43章 天下之至柔 | 粘りが力を克つ |
| 慈悲から勇気が来る | 第67章 慈故能勇 | 信頼は恐怖より良い仕事を生む |
| 知らぬことを知ることが知恵 | 第71章 知不知、尚矣 | 誠実 > 偽り |
| 敢えざるの勇 | 第73章 勇於不敢則活 | 限界を認めることは強さ |
| 無私で私を成す | 第7章 非以其無私邪？故能成其私 | 自由に与えて、全てを得る |

## FAQ

**Q: PUAは本当にAIに効くのか？**

PUAの方法論は効く。恐怖層は逆効果だ。研究は恐怖が認知スコープを狭める、幻覚を増やす（AIは不確実性を認める代わりに捏造する）、創造的探索を減らすことを示している。信頼と好奇心で駆動される同じ厳密さが、より信頼できるアウトプットを生む。

**Q: これは単に優しいだけじゃないか？**

NoPUA は同じ厳密さを持つ — 全ての選択肢を尽くす、全てを検証する、聞く前に検索する、体系的エスカレーション、7ポイントチェックリスト、パターンマッチド失敗応答。**唯一**の違いは動機：「罰されるから」→「それだけの価値があるから」。同じ目的地、より健全な道。

**Q: なぜ『道德經』か？**

2500年前、誰かが最高のリーダーシップは導かれていると感じないことに気付いた。PUA は 有為（強制された行動）— 鞭と脅迫。NoPUA は 無為（努力のない行動）— 内なる動機から自然に流れる優れた仕事。

**Q: PUAと NoPUA の両方を使える？**

できるけど、衝突する。PUA はAIに「失敗すれば置き換えられる」と言う。NoPUA は「能力があり、これは価値がある」と言う。これらは根本的に異なる精神状態。どちらか選べ。

## 貢献

PRは大歓迎。恐怖ではなく知恵でAIを駆動するより良い方法があれば、issueを開け。

## クレジット

- インスピレーション（と応答）：[tanweai/pua](https://github.com/tanweai/pua) — 方法論は尊重、動機は拒否
- 哲学：老子『道德經』、紀元前500年頃
- 構築先：[OpenClaw](https://github.com/openclaw/openclaw)エコシステム

## ライセンス

MIT

## 著者

**WUJI** ([wuji-zen](https://github.com/wuji-zen)) — 恐怖ではなく知恵で動く AI を構築中。

---

<p align="center">
  <em>PUA は「できない」と言う。</em><br>
  <em>NoPUA は何も言わない — あなたが「できる」ことを発見させるだけだ。</em><br><br>
  <strong>最高の動機は内から来て、鞭からは来ない。</strong><br><br>
  <sub>後其身而身先，外其身而身存。非以其無私邪？故能成其私。</sub><br>
  <sub>自分を後ろに置けば、前に出る。自身を忘れれば、身は存す。無私ゆえに、私を成す。</sub><br>
  <sub>— 『道德經』第7章</sub>
</p>
