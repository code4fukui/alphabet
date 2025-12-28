# alphabet opendata

- [alphabet.csv](alphabet.csv)

## license

- CC0 (PUBLIC DOMAIN)

## usage

```js
import { CSV } from "https://js.sabae.cc/alphabet.csv";

const data = await CSV.fetchJSON("https://code4fukui.github.io/alphabet/alphabet.csv");

// アルファベット大文字全部 26文字
console.log(data.map(i => i.alphabet).join(""));
```

