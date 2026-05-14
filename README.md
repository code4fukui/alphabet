# alphabet

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

## Features
- Provides a CSV file containing the English alphabet and their Japanese pronunciations.

## Data
The `alphabet.csv` file contains the following data:

- `alphabet`: The uppercase English alphabet (A-Z)
- `alphabet_low`: The lowercase English alphabet (a-z)
- `alphabet_jp`: The Japanese pronunciation of each English letter

## Usage

```js
import { CSV } from "https://js.sabae.cc/CSV.js";

const data = await CSV.fetchJSON("https://code4fukui.github.io/alphabet/alphabet.csv");

// Get the full uppercase English alphabet
console.log(data.map(i => i.alphabet).join(""));

// Get the full Japanese pronunciations of the alphabet
console.log(data.map(i => i.alphabet_jp).join(""));
```

## License
This project is released into the public domain under the [CC0 (PUBLIC DOMAIN)](https://creativecommons.org/publicdomain/zero/1.0/) license.