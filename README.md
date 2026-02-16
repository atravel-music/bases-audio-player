# Bases Audio Player Plugin

An Obsidian plugin that automatically adds audio players to Bases views for your Music properties.

## ⚡ Quick Start

### What you need:
- An Obsidian vault
- Audio files (.mp3, .wav, .ogg, .m4a) in your vault

### Installation in 4 steps:

1. **Copy all files** to `.obsidian/plugins/bases-audio-player/` in your vault

2. **Activate the plugin** in Obsidian:
   - Settings → Community Plugins → Bases Audio Player (turn on)

3. **Done!** Open a Bases view with a Music property and see the audio players appear

## 📝 Usage

Make sure your frontmatter looks like this:

```yaml
---
Music: [[my-music.mp3]]
---
```

Open a Bases view (table or card) and the audio link automatically becomes a player!

## 🎵 Features

- ✅ Works in table view
- ✅ Works in card view  
- ✅ Automatic detection of audio files
- ✅ Supports .mp3, .wav, .ogg, .m4a
- ✅ Shows filename below the player (table view)
- ✅ Centered overlay on cover art (card view)
- ✅ Beautiful outlined SVG play/pause icons
- ✅ Automatic pause of other players when starting new one

## 📦 Files

- `main.js` - Plugin code
- `manifest.json` - Plugin metadata
- `README.md` - Complete installation instructions
- `styles.css` - stylesheet

## Supported Formats

- `.mp3`
- `.wav`
- `.ogg`
- `.m4a`

## Troubleshooting

### Audio player is not shown

1. **Check if the plugin is active:**
   - Settings → Community Plugins → "Bases Audio Player" is turned on

2. **Check the file path:**
   - Make sure the audio file actually exists in your vault
   - The path in the frontmatter must be a valid wikilink: `[[file.mp3]]`

3. **Reload Obsidian:**
   - Cmd/Ctrl + R to reload Obsidian

4. **Check the console:**
   - Open Developer Tools (Cmd/Ctrl + Shift + I)
   - Look in the Console tab for error messages
  
## Technical Details

The plugin works by:
1. Monitoring the DOM for Bases views
2. Detecting links to audio files
3. Replacing them with HTML5 `<audio>` elements
4. Using the Obsidian vault adapter for correct file paths

---

Made with ❤️ for Obsidian Bases users
