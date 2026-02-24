# drumkit-kits

Sample drum kits for [drumkit](https://github.com/backmeupplz/drumkit) — the low-latency TUI MIDI drum sampler for Linux.

This repo is kept separate from the main drumkit repo to keep it light. Binary WAV files bloat git history, so they live here instead.

## Included Kits

- **freepats-gm** — General MIDI drum kit from the [FreePats](https://freepats.zenvoid.org/) project, with velocity layers and round-robin variations

## Usage

### As a git submodule (recommended)

If you cloned drumkit without `--recursive`:

```bash
cd drumkit
git submodule update --init
```

The kits will appear in `./kits/` and drumkit will find them automatically.

### Manual download

Download or clone this repo and point drumkit at it:

```bash
drumkit play --kits-dir /path/to/drumkit-kits
```

Or copy individual kit folders to `~/.local/share/drumkit/kits/`.

## Adding Your Own Kits

See the [drumkit README](https://github.com/backmeupplz/drumkit#sample-library-structure) for the naming convention.

## License

The WAV samples are from the [FreePats](https://freepats.zenvoid.org/) project and are available under their respective open licenses. See the FreePats website for details.
