# alphabet

## 機能
- 英語のアルファベットとその日本語での発音を含むCSVファイルを提供します。

## データ
`alphabet.csv` ファイルには以下のデータが含まれています:

- `alphabet`: 大文字の英語アルファベット (A-Z)
- `alphabet_low`: 小文字の英語アルファベット (a-z)
- `alphabet_jp`: 各英語アルファベットの日本語での発音

## 使い方

```js
import { CSV } from "https://js.sabae.cc/CSV.js";

const data = await CSV.fetchJSON("https://code4fukui.github.io/alphabet/alphabet.csv");

// 大文字の英語アルファベットをすべて取得
console.log(data.map(i => i.alphabet).join(""));

// アルファベットの日本語発音をすべて取得
console.log(data.map(i => i.alphabet_jp).join(""));
```

## ライセンス
このプロジェクトは [CC0 (PUBLIC DOMAIN)](https://creativecommons.org/publicdomain/zero/1.0/) ライセンスの下、パブリックドメインとして公開されています。
