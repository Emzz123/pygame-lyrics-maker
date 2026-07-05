# LSS Python Lyrics

A fullscreen Python/Pygame lyric display tool for building simple karaoke-style word animations.

The current script is:

- `python-lyrics/Misskonaikaw.py`

## Features

- Type or paste lyrics word by word.
- Pick text colors.
- Add effects like wave, flash, star particles, burst, glow, groups, and notes.
- Use image or video backgrounds for the menu and display screens.
- Present lyrics fullscreen and advance them one word at a time.

## Requirements

- Python 3
- `pygame`

Optional packages:

- `pyperclip` for paste support with `Ctrl+V`
- `opencv-python` and `numpy` for video backgrounds

Install the packages with:

```bash
pip install pygame pyperclip opencv-python numpy
```

## Run

From the project folder:

```bash
python python-lyrics/Misskonaikaw.py
```

## Basic Controls

Menu:

- `START` opens the lyric display screen.
- `EDIT` opens the lyric editor.
- `BACKGROUND` opens background settings.
- `FULLSCREEN` / `WINDOWED` switches screen mode.
- `EXIT` closes the app.

Editor:

- Type a word, then press `Space` to confirm it.
- Press `Enter` to finish editing and return to the menu.
- Press `Backspace` to delete text.
- Press `Ctrl+V` to paste lyrics if `pyperclip` is installed.
- Click a word to edit it.
- Use the effect buttons to apply effects to the selected word.
- Hold `Ctrl` and click words to group them.

Display:

- Press `Space` to show the next word.
- Press `Backspace` to reset the display.
- Press `Esc` to return to the menu.

## Note About Start

Clicking `START` does not immediately show the first lyric word. It opens the display screen in a waiting state. Press `Space` after clicking `START` to begin showing the lyrics.

## Troubleshooting

If the app feels slow, try switching to windowed mode or removing heavy video backgrounds. Video backgrounds need `opencv-python` and `numpy`; without them, image backgrounds still work.
#
