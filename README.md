# Junkbin.io — Translations

This repository contains the translation files for [Junkbin.io](https://junkbin.io), the community-driven e-waste and right-to-repair component database.

## Contribute

The easiest way to contribute translations is through **Weblate**:

[![Translation status](https://hosted.weblate.org/widget/junkbin-io/frontend-ui/svg-badge.svg)](https://hosted.weblate.org/projects/junkbin-io/)

👉 **[Translate on Weblate](https://hosted.weblate.org/projects/junkbin-io/)**

No coding or Git knowledge required — Weblate provides a web UI where you can translate strings directly in your browser.

## Languages

| Code | Language | Frontend UI | Backend strings |
|------|----------|-------------|-----------------|
| `en` | English | Source | Source |
| `fr` | Français | Machine-translated | Machine-translated |
| `es` | Español | Machine-translated | Machine-translated |
| `pt` | Português | Machine-translated | Machine-translated |
| `de` | Deutsch | Machine-translated | Machine-translated |
| `it` | Italiano | Machine-translated | Machine-translated |
| `nl` | Nederlands | Machine-translated | Machine-translated |
| `pl` | Polski | Machine-translated | Machine-translated |
| `cs` | Čeština | Machine-translated | Machine-translated |
| `sk` | Slovenčina | Machine-translated | Machine-translated |
| `hr` | Hrvatski | Machine-translated | Machine-translated |
| `sr` | Srpski | Machine-translated | Machine-translated |
| `sl` | Slovenščina | Machine-translated | Machine-translated |
| `ru` | Русский | Machine-translated | Machine-translated |
| `uk` | Українська | Machine-translated | Machine-translated |
| `ro` | Română | Machine-translated | Machine-translated |
| `hu` | Magyar | Machine-translated | Machine-translated |
| `tr` | Türkçe | Machine-translated | Machine-translated |

## File structure

```
frontend/locales/{lang}/translation.json   ← React UI strings (react-i18next)
backend/locale/{lang}/LC_MESSAGES/django.po ← Email templates & validation errors (Django gettext)
```

## How it works

- **Weblate → main repo**: When translations are committed here via Weblate, a GitHub Action automatically opens a pull request on the main Junkbin.io repository for review.
- **Main repo → here**: When new source strings are added to Junkbin.io, they are automatically synced to this repository so Weblate picks them up.

## Manual contribution (advanced)

If you prefer to contribute via Git:

1. Fork this repository
2. Edit `frontend/locales/{your-lang}/translation.json` — change the values, never the keys
3. For backend strings, edit `backend/locale/{your-lang}/LC_MESSAGES/django.po` — fill in the empty `msgstr` lines
4. Open a pull request

See [CONTRIBUTING_TRANSLATIONS.md](https://github.com/X9X0/junkbin.io/blob/main/docs/CONTRIBUTING_TRANSLATIONS.md) for a full guide.

## License

Translation content is licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
