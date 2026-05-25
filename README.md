# sawnd

`sawnd` is a terminal-based MP3 player with synchronized lyrics support, built with Go using [Bubble Tea](https://github.com/charmbracelet/bubbletea) for the TUI and [Beep](https://github.com/faiface/beep) for audio playback.

## Features

- **TUI Interface**: A clean, responsive terminal interface with a progress bar.
- **Lyrics Sync**: Supports `.lrc` files to display lyrics in sync with the music.
- **Playback Control**: Pause/Resume and Seek functionality.
- **Volume Control**: Adjust volume directly from the terminal.
- **Looping**: Option to loop the track a specific number of times or infinitely.

## Installation

Ensure you have [Go](https://golang.org/doc/install) installed.

```bash
go install github.com/zaater/sawnd@latest
```

*Note: Depending on your OS, you might need additional audio development libraries (e.g., `libasound2-dev` on Ubuntu/Debian).*

## Usage

```bash
sawnd <file.mp3> [OPTIONS]
```

### Options

- `-loop <n>`: How many loops, `-1` for infinitely (default 1).
- `-lrc <path>`: Path to the `.lrc` lyrics file.

### Controls

| Key | Action |
|-----|--------|
| `Space` | Toggle Pause/Play |
| `h` | Seek backward 10 seconds |
| `l` | Seek forward 10 seconds |
| `k` | Increase volume |
| `j` | Decrease volume |
| `q` / `Ctrl+C` | Quit |

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
