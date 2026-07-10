# skill-presentation

柔道整復師が立ち上げる「自律神経スクール」の集客を、他業種（塾・歯科医・小児科医・市役所）に **相互送客の提携** として持ちかけるための、商談台本＋想定問答を対話で作る自分専用スキル `writing-proposals` を収めたリポジトリ。

## 使い方（2通り）

### A. claude.ai（ブラウザ）で使う ― 推奨

1. このリポジトリの [`writing-proposals.zip`](writing-proposals.zip) をダウンロードする
2. claude.ai の **設定 > 機能（Capabilities）> スキル** を開き、zip をアップロードして登録する
3. 新規チャットで「**塾向けに集客協力の台本を作って**」のように依頼すると、スキルが起動して業種の確認から始まる

> 注意：GitHub のリポジトリURLをチャットに貼るだけでは、スキルは起動しません。

### B. Claude Code で使う

このリポジトリ（skill-presentation）を Claude Code で開き、`/writing-proposals` と打つか、「塾向けに集客協力の営業台本を作って」のように依頼すると起動します。

## 構成

```
.claude/skills/writing-proposals/
├── SKILL.md                     … スキル本体
└── references/
    ├── examples.md              … 模範台本例（塾・歯科医・市役所）
    └── output-quality.md        … 出力前の品質チェックリスト
writing-proposals.zip            … claude.ai スキル登録用パッケージ（上記と同内容）
```

スキルの中身を更新したときは、`.claude/skills/writing-proposals/` を修正してから `writing-proposals.zip` を作り直して差し替える。
