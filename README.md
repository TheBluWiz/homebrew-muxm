# homebrew-muxm

Homebrew tap for [MuxMaster](https://github.com/TheBluWiz/MuxMaster) (`muxm`) — a video encoding/muxing utility for Dolby Vision, HDR10, HLG, and SDR with format profiles.

## Install

```bash
brew install TheBluWiz/muxm/muxm
```

Or tap first, then install:

```bash
brew tap TheBluWiz/muxm
brew install muxm
```

Then run first-time setup:

```bash
muxm --install-completions   # tab completion for bash/zsh
```

## Optional dependencies

These are auto-disabled at runtime if missing. Install as needed:

```bash
brew install dovi_tool    # Dolby Vision RPU extraction/injection
brew install gpac         # DV container signaling verification (MP4Box)
brew install tesseract    # PGS subtitle OCR engine
```

For subtitle burn-in (`--sub-burn-forced`), ffmpeg needs libass:

```bash
brew tap homebrew-ffmpeg/ffmpeg
brew install homebrew-ffmpeg/ffmpeg/ffmpeg --with-libass
```

## Update

```bash
brew update
brew upgrade muxm
```

## Uninstall

```bash
muxm --uninstall-completions
muxm --uninstall-man
brew uninstall muxm
```

## More info

- **Documentation:** `man muxm` or `muxm --help`
- **Source:** [TheBluWiz/MuxMaster](https://github.com/TheBluWiz/MuxMaster)
- **Issues:** [GitHub Issues](https://github.com/TheBluWiz/MuxMaster/issues)
