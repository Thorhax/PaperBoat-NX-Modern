# PaperBoat
*Harbour Masters port of Paper Mario 64*

Project Lead:
* Caladius

Developers:
* Bass3l
* JeodC
* Caladius
* KiritoDv

## Website & Discord
Official Website: https://www.harbourmasters.org/

Official Discord: https://discord.gg/harbourmasters

*If you're having any trouble after reading through this `README`, feel free ask for help in the PaperBoat text channels. Please keep in mind that we do not condone piracy.*

# Quick Start

PaperBoat does not include any copyrighted assets.  You are required to provide a supported copy of the game.

### 1. Verify your ROM dump
US SHA1 Hash: `3837f44cda784b466c9a2d99df70d77c322b97a0`
You can verify you have dumped a supported copy of the game by using the compatibility checker at https://paperboat.equipment/.

### 2. Download PaperBoat from [Releases](https://github.com/HarbourMasters/PaperBoat/releases)

### 3. Launch the Game!
#### Windows
* Extract the zip
* Launch `paperboat.exe`

#### Linux
* Place your supported copy of the game in the same folder as the appimage.
* Execute `paperboat.appimage`. You may have to `chmod +x` the appimage via terminal.

#### macOS
* Run `paperboat.app`.
* When prompted, select your supported copy of the game.

#### Nintendo Switch
* Copy `switch/paperboat/` to `sdmc:/switch/paperboat/` on your microSD card.
* Place your supported copy of the game (`baserom.us.z64` or `pm64.o2r`) in `sdmc:/switch/paperboat/`.
* Launch `PaperBoat` via the Homebrew Menu (launching with title redirection / full RAM access recommended).

### 4. Play!

Congratulations, you are now sailing with PaperBoat! Have fun!

# Controls & Configuration

### Nintendo Switch Controls
| N64 | Nintendo Switch | In-Game Action |
| - | - | - |
| **A** | **A** | Jump, Confirm, Talk, Inspect |
| **B** | **B** | Hammer, Cancel |
| **Z** | **ZL** | Spin, Action Command |
| **L** | **L** | Party Member Ability |
| **R** | **ZR** / **R** | Party Member Wheel |
| **Start** | **+ (Plus)** | In-Game Pause Menu (Journal, Badges, Map) |
| **Control Stick** | **Left Analog Stick** | Move Mario |
| **C-Up** | **Right Stick Up** | Partner Hint (Goombario) |
| **C-Down** | **Right Stick Down** | Toggle HUD / Battle Items |
| **C-Left** | **Right Stick Left** | Switch Partner / Ability |
| **C-Right** | **Right Stick Right** | Partner Ability |
| **D-Pad** | **D-Pad** | Navigation / Menus |

### Port Menu & Navigation
| Switch Input | Action |
| - | - |
| **- (Minus)** | Toggle Port Menu (Settings, Enhancements, Cheats, Mods) |
| **D-Pad / Left Stick** | Navigate Menu Items |
| **A** | Select / Toggle Option |
| **B** | Back / Deselect |
| **Touchscreen** | Tap to navigate menus or touch buttons in handheld mode |

### Graphics Backends
Currently, there are three rendering APIs supported: DirectX 11 (Windows), OpenGL (all platforms), and Metal (macOS). You can change which API to use in the `Settings` menu of the menubar, which requires a restart.

If you're having an issue with crashing, you can also change the API manually in the `paperboat.cfg.json` file by finding the `"Backend": {` section and updating the backend ID and name. Be sure to use one of the valid values:

- `0` = DirectX 11 (default on Windows)
- `1` = OpenGL
- `2` = Metal (default on macOS)

# Custom Assets

Custom assets are packed in `.o2r` or `.otr` files. To use custom assets, place them in the `mods` folder.

If you're interested in creating and/or packing your own custom asset `.o2r`/`.otr` files, check out the following tools:
* [**retro - OTR and O2R generator**](https://github.com/HarbourMasters64/retro)
* [**fast64 - Blender plugin (Note that PM64 is not fully supported at this time)**](https://github.com/HarbourMasters/fast64)

# Development

If you want to manually compile PaperBoat, please consult the [building instructions](docs/BUILDING.md).

<a href="https://github.com/Kenix3/libultraship/">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./docs/poweredbylus.darkmode.png">
    <img alt="Powered by libultraship" src="./docs/poweredbylus.lightmode.png">
  </picture>
</a>

# Special Thanks:

This wouldn't have been possible without your amazing work:

* [The Paper Mario decomp team](https://github.com/pmret/papermario)
* [The Paper Mario DX team](https://github.com/bates64/papermario-dx)
