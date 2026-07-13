<p align="center">
  <img src="assets/logo.png" width="128" alt="Vestium logo">
</p>

<h1 align="center">Vestium</h1>

<p align="center"><b>The GTA V Clothing Studio — build, preview, repair and ship FiveM clothing packs like a pro.</b></p>

<p align="center">
  <a href="https://github.com/SensityTech/Vestium/releases/latest"><img src="https://img.shields.io/github/v/release/SensityTech/Vestium?label=download&color=7c5dfa" alt="Latest release"></a>
  <a href="https://github.com/SensityTech/Vestium/releases"><img src="https://img.shields.io/github/downloads/SensityTech/Vestium/total?color=7c5dfa" alt="Downloads"></a>
  <a href="https://discord.gg/rXbhzZdDVj"><img src="https://img.shields.io/badge/Discord-join-5865F2?logo=discord&logoColor=white" alt="Discord"></a>
</p>

<p align="center">
  <img src="assets/banner.png" width="720" alt="Vestium">
</p>

<p align="center"><sub><b>TRUSTED BY</b></sub></p>
<p align="center">
  <a href="https://cilyamods.tebex.io/" title="Cilya Mods"><img src="assets/partners/cilyamods.png" width="72" alt="Cilya Mods"></a>
</p>

---

## Download

Grab the latest **[Vestium-Setup.exe](https://github.com/SensityTech/Vestium/releases/latest)** (installer, auto-updates) or the portable build from the [releases page](https://github.com/SensityTech/Vestium/releases).

- **Windows 10/11 x64**
- Auto-updates: the app checks this repository and updates itself — install once, stay current.

## What is Vestium?

Vestium is a complete desktop studio for creating and managing GTA V addon clothing (FiveM first):

- **Import thousands of drawables in seconds** — names, genders, texture letters, physics, first-person models resolved automatically, content-deduplicated.
- **Animated 3D preview without launching the game** — full freemode ped, idle animations, live texture hot-swap, Photoshop live editing.
- **Optimization at scale** — real Blender LOD decimation, bulk texture re-encode (DXT/mips/pow2), parallel engine pool.
- **26+ live validations** before you ever hit build.
- **Byte-faithful FiveM builds** — addon collections AND replacement of real Rockstar DLCs, with DCT-compatible shop hashes so existing scripts and Tebex packages keep working.
- **Gen9/console safety** — reserved slots are scanned, locked and mirrored: your pack can never land on a dead index.
- **Repair tools** — re-open any compiled pack as an editable project, realign permuted texture letters by content hash, restore heels/flags from original packs.
- **`.vestfile` garment exchange** — export a complete garment as one portable file, bulk-import into any project with automatic pack placement.
- **Built-in Git collaboration** — LFS preconfigured, one-click private repo creation, team sync warnings.
- Bilingual **English/French**, dark & light themes, undo/redo everywhere.

## Translations

Vestium ships in English, French, Spanish, Russian, German, Portuguese,
Italian and Polish. The community dictionaries live in [`locales/`](locales/)
— spotted a bad translation or want to add your language? PRs are welcome,
see [locales/README.md](locales/README.md).

## Community

Join the **[Vestium Discord](https://discord.gg/rXbhzZdDVj)** — get help, share your packs, request features and follow updates.

## Issues & feedback

Found a bug or want a feature? [Open an issue](https://github.com/SensityTech/Vestium/issues) or ask on the [Discord](https://discord.gg/rXbhzZdDVj) — include your Vestium version and, when relevant, the console output (Ctrl+L in the app).

## Credits & acknowledgments

Vestium stands on the shoulders of the GTA modding community. Sincere thanks to:

- **[CodeWalker](https://github.com/dexyfex/CodeWalker)** by *dexyfex* — Vestium's engine vendors **CodeWalker.Core** to read and write RAGE formats (YDD, YTD, YMT, YLD, YCD, RPF). Vestium simply wouldn't exist without it.
- **[grzyClothTool](https://github.com/grzybeek/grzyClothTool)** by *grzybeek* — an excellent open-source clothing tool that inspired parts of Vestium's workflow. Vestium shares **no code** with it; everything is a clean-room reimplementation.
- **DurtyClothTool** — the reference clothing tool whose feature set Vestium set out to match and then go beyond. Used as functional inspiration and a format reference only — no code reused.

Built with **[three.js](https://threejs.org)** & **@react-three/fiber** (3D preview), **Magick.NET** (texture encoding), **Blender** (mesh decimation), **Electron**, **React**, **Vite** and **zustand**. Ships the **Manrope** typeface under the SIL Open Font License. Format knowledge comes from the FiveM / CitizenFX community and the clothing documentation at [docs.gta.clothing](https://docs.gta.clothing).

Vestium is an independent project and is not affiliated with, endorsed by, or associated with any of the above, nor with Rockstar Games or Take-Two Interactive.

## License

Vestium is proprietary software by SensityTech. This repository hosts the official builds and release notes only.
