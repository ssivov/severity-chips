# severity-chips

Severity badges for automated PR review comments. Each severity ships a light
and a dark SVG, embedded through `<picture>` so GitHub swaps the art with the
reader's theme.

<a><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/major_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/major_light.svg"><img align="top" valign="top" alt="Major" title="Major" src="https://raw.githubusercontent.com/ssivov/severity-chips/main/major_light.svg"></picture></a> <a><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/medium_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/medium_light.svg"><img align="top" valign="top" alt="Medium" title="Medium" src="https://raw.githubusercontent.com/ssivov/severity-chips/main/medium_light.svg"></picture></a> <a><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/minor_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/minor_light.svg"><img align="top" valign="top" alt="Minor" title="Minor" src="https://raw.githubusercontent.com/ssivov/severity-chips/main/minor_light.svg"></picture></a>

Glyphs are baked to outlines (Inter SemiBold, 12px) rather than set as `<text>`,
so a badge renders identically wherever it is proxied and depends on no font
being installed.

## Usage

Paste the snippet for the severity you want, then write the text straight after
it — each snippet ends with its own spacing so the chip does not crowd the
first word.

```html
<!-- Major -->
<a><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/major_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/major_light.svg"><img align="top" valign="top" alt="Major" title="Major" src="https://raw.githubusercontent.com/ssivov/severity-chips/main/major_light.svg"></picture></a>&nbsp;&nbsp;

<!-- Medium -->
<a><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/medium_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/medium_light.svg"><img align="top" valign="top" alt="Medium" title="Medium" src="https://raw.githubusercontent.com/ssivov/severity-chips/main/medium_light.svg"></picture></a>&nbsp;&nbsp;

<!-- Minor -->
<a><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/minor_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ssivov/severity-chips/main/minor_light.svg"><img align="top" valign="top" alt="Minor" title="Minor" src="https://raw.githubusercontent.com/ssivov/severity-chips/main/minor_light.svg"></picture></a>&nbsp;&nbsp;
```
