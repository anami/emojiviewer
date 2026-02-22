# Emoji Grid

A single-page emoji browser and copy tool. Click any emoji to copy it as an HTML character code (or Unicode, or raw emoji). Tone-able emojis open a skin tone picker.

**Live:** [anami.github.io/emojiviewer](https://anami.github.io/emojiviewer)

## Features

- Search by name, emoji, U+ code, group, or subgroup
- Filter by Unicode group and subgroup
- Copy as HTML hex entities, HTML decimal entities, Unicode (`U+…`), or raw emoji
- Skin tone picker for supported emojis
- Adjustable emoji size
- Keyboard navigation (arrow keys, `\` to toggle sidebar)

## Running locally

Requires a static file server (the app fetches `emoji-test.txt` over HTTP):

```bash
python3 -m http.server 8080
```

or 
```bash
npx serve -l 8080
```

or 
```bash
php -S localhost 8080
```



Then open `http://localhost:8080`.

## Data source

Emoji data comes from the Unicode Consortium's [`emoji-test.txt`](https://unicode.org/Public/emoji/latest/emoji-test.txt) (currently Unicode 17.0). To update, replace `emoji-test.txt` with a newer version from the same URL.
