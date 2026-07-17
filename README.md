# AO3 Tooltip Formatter

A single-page tool that converts plain-text shorthand into the HTML tags used by [Simbeline's tooltips Work Skin](https://archiveofourown.org/works/30290274) on AO3.

**Live tool:** https://k0terina-ao3.github.io/ao3-tooltip/

## What it does

Write `(visible text;[hover text])` anywhere in your draft, paste the whole chapter in, and it converts only the tooltip markers into the `<span>` tags the Work Skin targets — everything else is left untouched.

Optionally, it can also convert simple markdown-style formatting:

- `**text**` → bold
- `*text*` → italic
- `~~text~~` → strikethrough
- `\*` / `\~` → escaped, literal character

Nothing typed into the page is sent anywhere or saved — all conversion happens client-side in the browser.

Note: this tool only generates the tags. For the hover effect to work on AO3, you still need to add the CSS from Simbeline's Work Skin to your fic's Work Skin.

## Development

It's a single static `index.html` with no build step or dependencies — open it directly in a browser to work on it.
