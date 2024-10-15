# 数学の樹 webサイト

[数学の樹トップページ](https://arbormathematica.github.io/tree-of-math-project/)

## 記事の書き方

1. ターミナル（下の画面）に`git pull`と入力する。
2. ルートフォルダにあるtemplate.mdを書きたい記事の属するフォルダにコピーする。
3. コピーしたtemplate.mdの以下を改変し、保存する。
   - ファイル名
   - タイトル
   - 日付
   - author name
   - category, tag
   - 記事の概要
   - 内容
4. ターミナル（下の画面）に`hugo serve`と入力し、プレビューを見る。プレビューは`http`から始まるリンクを`ctrl+クリック`することで開くことができる。
5. 問題がなければ、左側のグラフのマークをクリックして開く画面に更新内容を表すメッセージをいれ、コミットする。その後もう一度同じボタンで同期をする。

## markdown記法について

- *強調*（斜体）：`*強調*`
- **強い強調**（太字）：`**強い強調**`
- 箇条書き：`- 箇条書き`
- 番号付き箇条書き：`1. 箇条書き`
- セクションのタイトル：`## タイトル`
- サブセクションのタイトル：`### タイトル`
- 行内数式：`$数式$`または`\(数式\)`
- ディスプレイ数式：`$$数式$$`または`\[数式\]`

## 定理環境について

- 定義：`{{% def タイトル %}}`と`{{% /def %}}`で囲む
- 定理：`{{% thm タイトル %}}`と`{{% /thm %}}`で囲む
- 命題：`{{% prop タイトル %}}`と`{{% /prop %}}`で囲む
- 補題：`{{% lem タイトル %}}`と`{{% /lem %}}`で囲む

## category, tagの指針

### category

- 必ず分野名を入力する。
  - 例：代数学、幾何学、解析学
- より詳細な分野があったほうが良い場合は、それも入力する。
  - 例：多様体、群論

### tag

- その記事のカテゴリーを入力する。
  - 主に、定義、定理、命題、補題のいずれかを選んで用いる。

## その他

- vscodeに[Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)、[markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)を入れることを推奨する。
