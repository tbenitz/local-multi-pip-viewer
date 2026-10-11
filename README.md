# Local Multi-PiP Viewer

A pure local HTML tool for watching multiple video sources at once. Combine screen/tab/window captures with local video files and playlists. Floating Picture-in-Picture windows stay inside the page so everything is visible when you cast or share the browser tab.

No server required. Open the HTML file in Chrome/Edge (Chromebook compatible). Screen capture works best over a secure context, but the file itself is fully self-contained.

## Features

- Up to 5 simultaneous sources (configurable)
- Screen, tab, or window capture via the browser picker
- Local video files (single or multi-file playlists)
- Playlists that play through all videos and can loop the whole list
- Large main video + draggable/resizable floating PiPs
- Promote any PiP to main (positions are preserved on swap)
- Independent mute/volume per source
- Clean Fullscreen mode that hides all UI for casting
- Click a PiP in clean mode to make it main
- Hover controls in clean mode that auto-hide after mouse inactivity
- Settings: max sources, PiP size, snap-to-grid, auto-mute, accent color, hover delay
- Arrange button, cycle main, renameable labels

## How to Use

1. Download `index.html` (or clone the repo) and open it in Chrome or Edge.
2. **Add a screen capture**: Click **+ Capture**, choose options, then pick a tab, window, or screen.
3. **Add local videos**: Click **+ Video File**.
   - One file → loopable single video source.
   - Multiple files → creates a playlist. Open **Playlists** to start it and toggle loop.
4. The first source becomes the main video. Additional sources appear as floating PiPs.
5. **Move / resize PiPs**: Drag the header or video area. Resize from the bottom-right corner. Works in both normal and Clean Fullscreen modes.
6. **Make a PiP the main video**: Click the **Main** button, its chip in the tray, or (in Clean Fullscreen) click the PiP itself. The previous main takes the exact spot the promoted PiP occupied.
7. **Clean Fullscreen**: Click the button or press `F`. All UI hides so casting the tab shows only the videos. Press `Esc` or `F` to exit.
8. **Playlist controls**: Loop on = play all videos then restart. Loop off = play through once. Use Next to advance manually.
9. **Mute / volume**: Per-source buttons and sliders. Hover controls appear in Clean Fullscreen and disappear after inactivity.

## Keyboard Shortcuts

- `F` — Toggle Clean Fullscreen
- `Esc` — Exit Clean Fullscreen / close modals
- `Ctrl/Cmd + N` — New capture

## Tips

- Screen capture requires a secure context on some devices. If the picker fails when opening the file directly, try a quick local server or open via a Chromebook Linux environment.
- Only one OS-level Picture-in-Picture window can be active at a time; this tool uses in-page floating windows so multiple sources stay visible when casting.
- Everything runs locally. No data leaves your browser.

## Live Demo

If GitHub Pages is enabled, the live version is at the Pages URL for this repository.

## License

MIT — free to use and modify.
