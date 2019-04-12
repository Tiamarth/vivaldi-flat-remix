# vivaldi-flat-remix

This is a custom css file that integrates Vivaldi's interface with [Flat Remix,](https://github.com/daniruiz/flat-remix-gtk) by applying the correct window buttons in Vivaldi's css.

## Installation (Linux)
**Vivaldi Stable**
```bash
git clone https://github.com/Tiamarth/vivaldi-flat-remix.git && cd vivaldi-flat-remix
mv flat-remix.css /opt/vivaldi/resources/vivaldi/style/
mv flat-remix /opt/vivaldi/resources/vivaldi/style/
sed -i 's/  <\/head>/    <link rel="stylesheet" href="style\/flat-remix.css" \/>\n  <\/head>/' "/opt/vivaldi/resources/vivaldi/browser.html"
```
**Vivaldi Snapshot**
```bash
git clone https://github.com/Tiamarth/vivaldi-flat-remix.git && cd vivaldi-flat-remix
mv flat-remix.css /opt/vivaldi-snapshot/resources/vivaldi/style/
mv flat-remix /opt/vivaldi-snapshot/resources/vivaldi/style/
sed -i 's/  <\/head>/\n<link rel="stylesheet" href="style\/flat-remix.css" \/>\n  <\/head>/' "/opt/vivaldi-snapshot/resources/vivaldi/browser.html"
```

| Flat Remix:                      | Flat Remix Dark:                 | Flat Remix Darker:               | Flat Remix Darkest:              |
| -------------------------------- | -------------------------------- | -------------------------------- | -------------------------------- |
| Background: #ffffff              | Background: #2f343f              | Background: #ffffff              | Background: #000000              |
| Foreground: #000000              | Foreground: #ffffff              | Foreground: #000000              | Foreground: #ffffff              |
| Highlight: #367bf0               | Highlight: #367bf0               | Highlight: #367bf0               | Highlight: #367bf0               |
| Accent: #e6e6e6                  | Accent: #434854                  | Accent: #1a1a1a                  | Accent: #1a1a1a                  |
| [x] Transparent Tabs             | [x] Transparent Tabs             | [x] Transparent Tabs             | [x] Transparent Tabs             |
| [ ] Apply Accent Color to Window | [ ] Apply Accent Color to Window | [x] Apply Accent Color to Window | [ ] Apply Accent Color to Window |
| Corner Rounding: 2px             | Corner Rounding: 2px             | Corner Rounding: 2px             | Corner Rounding: 2px             |

Note that corner rounding in the above table is really more of a suggestion than a requirement for the purposes of integrating Vivaldi with Flat Remix. The actual gtk theme has varying border radius depending on the kind of ui element. For window borders and toolbars and such, the radius is usually very small. For ui buttons and input fields, the radius is usually very large. So set it to whatever you prefer.

**Need more help?** Get in touch!
- join my [Discord server](https://discord.gg/ZfDP2ZV)
- [Create an issue here on GitHub](https://github.com/Tiamarth/vivaldi-flat-remix/issues/new)
- [Email me](mailto:jontiamac@gmail.com)
