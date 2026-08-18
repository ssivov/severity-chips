# severity-chips

Severity badges for automated PR review comments. Two SVGs per severity — a
light and a dark variant — embedded with `<picture>` so GitHub swaps them with
the reader's theme.

| Severity | Light | Dark |
| --- | --- | --- |
| Major | ![Major](major_light.svg) | ![Major](major_dark.svg) |
| Medium | ![Medium](medium_light.svg) | ![Medium](medium_dark.svg) |
| Minor | ![Minor](minor_light.svg) | ![Minor](minor_dark.svg) |

Glyphs are baked to paths (Inter SemiBold, 12px), so the badge renders
identically wherever it is proxied, with no font dependency.

## Usage

```html
<a><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/major_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/major_light.svg"><img align="top" valign="top" alt="Major" title="Major" src="https://raw.githubusercontent.com/ssivov/severity-chips/main/major_light.svg"></picture></a>
```
