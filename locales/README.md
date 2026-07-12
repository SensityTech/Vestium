# Vestium translations

Help translate Vestium into your language! Every release of the app ships the
latest validated snapshot of the dictionaries in this folder.

## How it works

- **`en.json` is the reference** — it is generated from the app source and
  contains every key the UI uses. Do not edit it (or `fr.json`): both are
  maintained with the app and overwritten on every sync.
- Every other file (`es.json`, `ru.json`, `de.json`, `pt.json`, `it.json`,
  `pl.json`, …) is a **community dictionary**: same keys, translated values.
  The initial versions were machine-assisted — corrections are very welcome.
- A dictionary may be **partial**: any missing key simply falls back to
  English in the app. Translate what you can.

## Contributing

1. Fork this repository and edit (or create) `locales/<code>.json`.
2. Keep the rules below, then open a pull request. A CI check validates your
   file automatically.

### Rules

- The file must be **valid JSON** (UTF-8, no BOM, no comments, no trailing
  commas).
- Only use keys that exist in `en.json` — unknown keys are rejected.
- **Placeholders are sacred**: tokens like `{name}`, `{count}`, `{percent}`,
  `{error}` must appear in your translation exactly as they appear in the
  English value (the words inside braces are code, never translate them).
- Keep domain terms untouched: GTA V, FiveM, DLC, YMT/YTD/YDD/YLD, LOD,
  gen9, drawable, slot names (jbib, uppr, lowr, accs…), Blender, Photoshop,
  Git, dummy, addon/pack/bundle, `.vestfile`.
- Button labels stay short; match the tone of a professional desktop app.

## Adding a new language

Open an issue (or a PR with the new `<code>.json`) using the two-letter
ISO 639-1 code. The app team wires the language into the picker (with its
flag) in the next release.
