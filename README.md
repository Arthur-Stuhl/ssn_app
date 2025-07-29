# Social Stream Ninja Standalone (ssapp)

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Build Status](https://github.com/steveseguin/ssapp/workflows/Build%20SS%20App%20for%20Linux/badge.svg)](https://github.com/steveseguin/ssapp/actions)

An Electron-based standalone application for [Social Stream Ninja](https://github.com/steveseguin/social_stream), providing better performance and stability than browser-based capture for streaming applications like OBS.

## Features

- 🎮 **Native Performance** - Better CPU/GPU efficiency compared to browser capture
- 🔌 **Direct OBS Integration** - Capture social media chats without browser overhead
- 💬 **Multi-Platform Support** - YouTube, Twitch, TikTok, and more
- 🎨 **Customizable Overlays** - Full styling control for your streams
- 🔊 **Text-to-Speech** - Built-in TTS with Kokoro-82M model
- 🛠️ **Event Flow System** - Create custom automation workflows

## Download

Download the latest release for your platform from the [Releases](https://github.com/steveseguin/ssapp/releases) page.

## Building from Source

### Prerequisites

- Node.js 18 or higher
- npm 8 or higher
- Python (for native module compilation)

### Development

```bash
# Clone the repository
git clone https://github.com/steveseguin/ssapp.git
cd ssapp

# Install dependencies
npm install

# Run in development mode
npm run start2
```

### Building

```bash
# Windows
npm run build:win32

# macOS (x64 and arm64)
npm run build:darwin

# Linux
npm run build:linux

# Raspberry Pi
npm run build:rpi
```

## Usage

1. Launch the application
2. Load Social Stream Ninja or your custom social stream URL
3. Configure your chat sources
4. Add the window capture to OBS

For detailed usage instructions, visit the [Social Stream Ninja documentation](https://socialstream.ninja/manual).

## Configuration

The app stores configuration in:
- Windows: `%APPDATA%/socialstream/`
- macOS: `~/Library/Application Support/socialstream/`
- Linux: `~/.config/socialstream/`

## Code Signing

Official releases are signed. You can verify the authenticity using the included `code-signing-cert.pem` file. See [CODE_SIGNING.md](CODE_SIGNING.md) for details.

## Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## Related Projects

- [Social Stream Ninja](https://github.com/steveseguin/social_stream) - The web application and Chrome extension
- [VDO.Ninja](https://github.com/steveseguin/vdo.ninja) - WebRTC live streaming tool

## Support

- 📖 [Documentation](https://socialstream.ninja/manual)
- 💬 [Discord Community](https://discord.socialstream.ninja)
- 🐛 [Report Issues](https://github.com/steveseguin/ssapp/issues)

## Acknowledgments

- Built with [Electron](https://www.electronjs.org/)
- TTS powered by [Kokoro-82M](https://huggingface.co/hexgrad/Kokoro-82M)
- Part of the [VDO.Ninja](https://vdo.ninja) ecosystem