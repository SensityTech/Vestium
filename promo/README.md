# Recommended creators (in-app popup)

`promo.json` drives the **"Recommended creators"** popup shown when Vestium
starts. The app fetches this file (and the images it references) directly from
this repository on every launch — **editing it here updates every install,
no release needed**. Content is cached locally so the popup also works offline.

## Format

```jsonc
{
  "version": 1,               // must stay 1
  "banner": null,             // or: { "image": "promo/banner.png", "url": "https://..." }
  "creators": [
    {
      "id": "cilyamods",                          // unique slug
      "name": "Cilya Mods",                       // display name
      "taglines": {                               // optional one-liner per language
        "en": "Premium FiveM clothing packs",
        "fr": "Packs de vêtements FiveM premium"
      },
      "logo": "assets/partners/cilyamods.png",    // image path INSIDE this repo
      "url": "https://cilyamods.tebex.io/"        // store link (https only)
    }
  ]
}
```

## Rules (enforced by the app)

- `url` links must be **https**; anything else drops the entry.
- `logo` / `banner.image` must be **paths inside this repository**
  (png/jpg/webp/gif, max 2 MB) — remote URLs are ignored.
- At most **12 creators** are shown.
- `banner` is the ad slot at the top of the popup: set it to an object to
  activate it, keep `null` to hide the slot.
- A malformed entry is skipped silently; the rest keeps working.

Put partner logos in [`assets/partners/`](../assets/partners/).
