# skill-presentation

柔道整復師が立ち上げる「自律神経スクール」の集客を、他業種（塾・歯科医・小児科医・市役所）に **相互送客の提携** として持ちかけるための、商談台本＋想定問答を対話で作る自分専用スキル `writing-proposals` を収めたリポジトリ。

## 使い方（3通り）

### A. claude.ai（ブラウザ）で使う ― 推奨・貼ったら動く

[`paste-to-run.md`](paste-to-run.md) の**中身をまるごとコピー**し、claude.ai の新規チャットに貼って送信します。貼った直後から「対象業種の確認 → 商談台本＋想定問答の作成」が始まります。

> 注意：**GitHub のリポジトリURLを貼るだけでは、claude.ai でスキルは起動しません。** スキルは「意図（依頼文）」に反応して動く仕組みで、リポジトリは保管場所であってトリガーではないためです。`paste-to-run.md` は、その中身を貼れば同じ挙動になるよう1ファイルに自己完結させたものです。

### B. Claude Code で使う

このリポジトリ（skill-presentation）を Claude Code で開き、`/writing-proposals` と打つか、「塾向けに集客協力の営業台本を作って」のように依頼すると起動します。スキル本体は [`.claude/skills/writing-proposals/`](.claude/skills/writing-proposals/) にあります。

### C. claude.ai にカスタムスキルとして登録する（任意）

利用中のプランがカスタムスキルの登録に対応していれば、`writing-proposals` をスキルとして導入し、依頼文で起動できます。

## 構成

```
.claude/skills/writing-proposals/
├── SKILL.md                     … スキル本体（Claude Code / スキル登録で使用）
└── references/
    ├── examples.md              … 模範台本例（塾・歯科医・市役所）
    └── output-quality.md        … 出力前の品質チェックリスト
paste-to-run.md                  … claude.ai 貼り付け用の自己完結版
```
