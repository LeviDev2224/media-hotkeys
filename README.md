# Media Hotkeys

**Control background music and videos without switching windows.**

## Why I Built This

I got tired of having to tab out of whatever I was working on just to pause a video, skip a song, or change the volume. I wanted a simple way to control media in the background without interrupting what I was doing, so I built this Python utility.

Media Hotkeys runs in the background and listens for global keyboard shortcuts, allowing you to control media while another application is in focus.

## Features

- Play or pause music and videos
- Skip to the next or previous track
- Increase or decrease system volume
- Mute or unmute audio
- Exit using a keyboard shortcut

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl + Alt + P` | Play / Pause |
| `Ctrl + Alt + Right` | Next Track |
| `Ctrl + Alt + Left` | Previous Track |
| `Ctrl + Alt + Up` | Volume Up |
| `Ctrl + Alt + Down` | Volume Down |
| `Ctrl + Alt + M` | Mute / Unmute |
| `Ctrl + Alt + Esc` | Exit Program |

## Installation

Designed for Windows. Requires Python 3.

**1. Clone the repository**

```bash
git clone https://github.com/LeviDev2224/media-hotkeys.git
cd media-hotkeys
```

**2. Install dependencies**

```bash
python -m pip install keyboard pyautogui
```

**3. Run the program**

```bash
python main.py
```

The program will remain active, listening for keyboard shortcuts, until you exit using `Ctrl + Alt + Esc`.

**Note:** Media controls depend on the application playing your music or video. Some programs might not respond to every command.

## How It Works

The script uses two Python libraries:

- **keyboard:** Registers global keyboard shortcuts that work even when another application is focused.
- **PyAutoGUI:** Sends media-control key commands to the operating system.

Together, these allow media playback to be controlled without manually switching to the media player.

## Technologies Used

- Python
- keyboard
- PyAutoGUI

## License

See [LICENSE](LICENSE) for details.
