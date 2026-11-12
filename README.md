# Img2Font

Turn a picture of letters or numbers into a font you can install. Img2Font is free and runs entirely in your browser. Your images are never uploaded.

**Try it:** https://moggle-khraum.github.io/Img2Font/

## Quick start

1. **Add an image.** Drop a PNG or JPG onto the page, or click the box to choose one. You can also pick a sample sheet from the "Try a sample sheet" menu.
2. **Type what's on the sheet.** In "What is on the sheet?", type the characters one row at a time, in the order they appear, from left to right and top to bottom. For example, `ABC` on one row and `abc` on the next.
3. **Check the outlines.** Each detected letter gets a blue box. If the boxes are wrong, adjust the darkness cut-off or drag a box around just the letters you want.
4. **Try your font.** Type in "Try some text" to preview it.
5. **Download.** Choose .ttf to install the font on a computer, or .woff for the web. "Copy CSS" gives you a ready-made `@font-face` rule with the font embedded.

## Tips for a good result

- Use dark ink on light paper, with letters spaced apart. Letters that touch will be merged into one shape.
- Keep the sheet flat and well lit. If the photo is tilted or shadowed, try the "Phone photo" sample to see how the settings handle it.
- Keep dots on i and j close to their letters, and make sure descenders such as g, j, p, q, and y are listed under "Characters that hang below the baseline."
- If the status says there are more shapes than characters, it usually means part of the sheet is being picked up as letters. Drag a box around just the letters.
- Use the spacing box under a letter to adjust the gap on each side of it. Leave it blank to use the general spacing.

## Controls

- **Undo** (or Ctrl+Z / Cmd+Z) steps back through your changes, including loading an image, slider moves, spacing edits, and clearing.
- **Clear** removes the image, resets the settings to their defaults, and clears the letter spacing. You can undo it.
- Your settings and letter layout are saved in your browser, so they're still there next time. Images are not saved.

## Offline use

Img2Font works without an internet connection once it has loaded once. Open the page in your browser and use the browser's "Install" or "Add to Home screen" option to keep it on your device.

## Files

- `index.html`: the whole app, with its styles and code. It works on its own.
- `sw.js`, `manifest.webmanifest`, `icon.svg`: optional helpers for offline use and installing. Img2Font still works without them.

## Limits

- Only basic characters are supported (the Unicode Basic Multilingual Plane). Characters outside that range are skipped.
- Very large photos may be slow on older phones. The page resizes images to at most 3000 pixels on the longest side.
- Connected cursive handwriting can't be split into letters yet. Write letters apart for best results.

## License

No license has been chosen yet. Add a `LICENSE` file before others reuse the code.
