# drumkit-kits

Sample drum kits for [drumkit](https://github.com/backmeupplz/drumkit) — the low-latency TUI MIDI drum sampler for Linux.

This repo is kept separate from the main drumkit repo to keep it light. Binary WAV files bloat git history, so they live here instead.

## Included Kits

| Kit | Style | Velocity Layers | Round Robins | Notes | Size | License |
|-----|-------|----------------|--------------|-------|------|---------|
| **freepats-gm** | General MIDI | up to 2 | up to 9 | 68 files | 18MB | GPL v3+ |
| **avl-black-pearl** | Acoustic rock | 5 | - | 128 files | 21MB | CC-BY-SA 3.0 |
| **virtuosity-jazz** | Contemporary jazz | up to 36 | up to 4 | 434 files | 227MB | CC0 |
| **linndrum** | 80s electronic / synth-pop | up to 3 | - | 29 files | 952KB | Public Domain |
| **personal-jesus-909** | Industrial electronic / TR-909 | 3 | 2 (clap) | 27 files | 2.7MB | Free non-commercial |
| **cats** | Cat meows & growls | - | - | 27 files | 9MB | CC0 |

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

## Credits

- **FreePats GM** — [freepats.zenvoid.org](https://freepats.zenvoid.org/)
- **AVL Black Pearl** — [bandshed.net/avldrumkits](http://www.bandshed.net/avldrumkits/)
- **Virtuosity Jazz** — [Virtuosity Drums](https://github.com/sfzinstruments/virtuosity_drums) by Versilian Studios / Karoryfer Samples (overhead mic position)
- **LinnDrum LM-2** — [Oramics/Sampled](https://oramics.github.io/sampled/DM/LM-2/) (Public Domain, sourced from machines.hyperreal.org)
- **Personal Jesus 909** — Roland TR-909 samples by Rob Roy / Rob Roy Recordings (1995), sourced from [drumkito.com](https://www.drumkito.com/sample-packs/roland-tr-909-sample-pack/). Free to copy/distribute, not for profit.
- **Cats** — Cat meow, growl, and roar samples by Joseph Sardin, sourced from [BigSoundBank](https://bigsoundbank.com/). CC0 / Public Domain.
