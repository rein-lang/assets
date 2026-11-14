# Rein assets

The single source of truth for Rein brand files. Other repos consume this repo as a git submodule and do not keep their own copies.

| File | Use |
| --- | --- |
| `logo.svg`, `logo-512.png`, `logo-256.png` | The Rein logo. |
| `mark.svg`, `mark-512.png` | The mark alone. |
| `circle.svg`, `circle-512.png` | The logo in a circle, for avatars. |
| `square.svg`, `square-512.png` | The logo in a square. |
| `icon-256.png` | App icon, used by the VS Code extension. |
| `favicon.svg`, `favicon.ico`, `apple-touch-icon.png` | Site icons for rein-lang.com. |

## Consumers

- [rein-lang.com](https://github.com/rein-lang/rein-lang.com): submodule at `assets/`; the site `public/` folders link to it.
- [vscode-rein](https://github.com/rein-lang/vscode-rein): submodule at `assets/`; the extension icon is `assets/icon-256.png`.
- [rein](https://github.com/rein-lang/rein): the README loads `logo.svg` by its raw URL, because GitHub does not render images from a submodule.

To add a consumer: `git submodule add https://github.com/rein-lang/assets.git assets`.
