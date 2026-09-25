<div align="center">

# Axiom Dotfiles

**A complete Hyprland desktop in one repository, set up from inside the desktop itself.**

💍 *One config to rule them all.*

Bar, overlay, launcher, notifications, lockscreen, OSD, theming and your Hyprland setup, all in one shell.<br>
It needs only `qs`, `python3` and `jq`.

[![Organization Followers](https://img.shields.io/github/followers/axiom-dotfiles?style=for-the-badge&logoColor=ebdbb2&labelColor=282828&label=Follow&color=458588)](https://github.com/axiom-dotfiles)
[![Stars](https://img.shields.io/github/stars/axiom-dotfiles/axiom?style=for-the-badge&logoColor=ebdbb2&labelColor=282828&color=d79921)](https://github.com/axiom-dotfiles/axiom)
[![Release](https://img.shields.io/github/v/tag/axiom-dotfiles/axiom?filter=v*&style=for-the-badge&logoColor=ebdbb2&labelColor=282828&label=Release&color=b8bb26)](https://github.com/axiom-dotfiles/axiom/tags)
[![Latest Commit](https://img.shields.io/github/last-commit/axiom-dotfiles/axiom?style=for-the-badge&logoColor=ebdbb2&labelColor=282828&color=98971a)](https://github.com/axiom-dotfiles/axiom)
<br>
[![Hyprland](https://img.shields.io/badge/Hyprland-0.55%2B-458588?style=for-the-badge&labelColor=282828)](https://hypr.land)
[![Quickshell](https://img.shields.io/badge/Quickshell-0.3.1%2B-b16286?style=for-the-badge&labelColor=282828)](https://quickshell.org)
[![License](https://img.shields.io/badge/License-MIT-689d6a?style=for-the-badge&labelColor=282828)](LICENSE)

[Features](#-why-axiom) · [Gallery](#-gallery) · [Quick start](#-quick-start) · [Roadmap](#%EF%B8%8F-roadmap)

</div>

https://github.com/user-attachments/assets/a53f62e0-e2bc-4834-a05f-92b6cb115c35

> [!TIP]
> Everything in this video was built from inside the shell: the settings, the bars, the overlay pages and the themes. No file was edited by hand, and switching between whole setups is one click.

## ✨ Why axiom

<table>
<tr>
<td width="33%" valign="top">

### 🛠️ Built in the shell
Your whole desktop is data, and the shell edits all of it. Drag widgets onto your bars and modules onto overlay pages, and watch them change live. Every option is on a Settings page generated from the config schema. You never write a config file.

</td>
<td width="33%" valign="top">

### 📦 Batteries included
The whole desktop is in one repository with one config. There's no separate bar, launcher, notification daemon, locker and theming tool to wire together. Beyond Hyprland and Quickshell it needs only `python3` and `jq`. Every other tool is optional and only turns on the feature that uses it.

</td>
<td width="33%" valign="top">

### 🛡️ Built not to break
A broken `config.json` never replaces the one that's running. Configs from older versions are migrated automatically, and saved snapshots are one click away. API keys are kept out of your config.

</td>
</tr>
<tr>
<td valign="top">

### 📊 Bars your way
Any number of bars, on any monitor and any edge. Each one can be solid, transparent, or split into floating pills that merge into the screen border. There are 20 widget types, and their popouts grow out of the bar.

</td>
<td valign="top">

### 🗂️ An overlay you design
Full-screen pages of cards, built from 24 modules: media, a mixer, system graphs, processes, weather, notes, quick toggles, AI chat and more. Each module adapts to the shape of its slot.

</td>
<td valign="top">

### 🎨 Wallpaper → theme → every app
It builds a base16 palette from your wallpaper in OKLCH, tuned to match the contrast of the hand-made themes. That palette then themes 18 apps: GTK, Qt, five terminals, Neovim, Helix, VS Code, btop, lazygit and more.

</td>
</tr>
<tr>
<td valign="top">

### 🤝 Fits your Hyprland config
axiom can apply itself at runtime and leave your files alone, write a file your config includes, or manage `hyprland.lua` for you, loading your own files after it.

</td>
<td valign="top">

### 🧭 Grid workspaces
Use workspaces 1 to N, or a grid on each monitor that you move around by row and column. A live overview lets you drag windows between workspaces. The bar, the map and your keybinds all follow the same layout.

</td>
<td valign="top">

### 🖥️ Multi-monitor, multilingual
Wallpapers and bars are set per monitor. Surfaces open on the primary monitor, the focused one, or all of them. The shell is in English and Japanese, and adding a language takes one JSON file.

</td>
</tr>
</table>

<div align="center">

**20** bar widgets · **24** overlay modules · **5** built-in pages · **10** hand-made themes · **18** app integrations · **3** lockscreen modes

</div>

<details>
<summary><b>…and the rest</b></summary>

- **Launcher:** searches apps (ranked by how often and how recently you use them), open windows, a calculator and the web. It also runs shell commands and controls the shell with `/` commands.
- **Notifications:** toasts, plus a notification center whose history survives reloads.
- **Per-app OSD:** the volume OSD follows the apps you choose, not only the master volume.
- **Your choice of lockscreen:** the built-in Wayland session lock (PAM), a themed hyprlock config that axiom generates, or your own locker.
- **Keybinds page:** lists every bind Hyprland knows, and edits axiom's own binds with conflict detection and key recording.
- **AI chat:** Anthropic, OpenAI, Gemini or any OpenAI-style API (Ollama and friends), streaming Markdown replies with thinking, saved conversations, presets and image attachments, with keys in your keyring.
- **Scriptable:** every surface can be controlled over IPC, so anything can drive it.

</details>

## 📸 Gallery

Both setups were built entirely in the shell. See the [axiom README](https://github.com/axiom-dotfiles/axiom#readme) for every page and popout.

<table>
<tr>
<td width="50%" align="center">
<img src="https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/assets/screenshots/desktop.webp" alt="Pill and transparent bars">
<br><sub><b>Pills</b>: floating pills and a transparent bar, down the sides</sub>
</td>
<td width="50%" align="center">
<img src="https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/assets/screenshots/desktop-b.webp" alt="A solid top bar">
<br><sub><b>Solid</b>: one bar across the top, same shell</sub>
</td>
</tr>
<tr>
<td align="center">
<img src="https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/assets/screenshots/overlay-home.webp" alt="The overlay">
<br><sub><b>The overlay</b>: pages of cards you lay out yourself</sub>
</td>
<td align="center">
<img src="https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/assets/screenshots/overlay-editor.webp" alt="Overlay editor">
<br><sub><b>Overlay editor</b>: drag modules onto a page</sub>
</td>
</tr>
<tr>
<td align="center">
<img src="https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/assets/screenshots/bar-editor.webp" alt="Bar editor">
<br><sub><b>Bar editor</b>: drag widgets and watch the bar change live</sub>
</td>
<td align="center">
<img src="https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/assets/screenshots/settings.webp" alt="Settings page">
<br><sub><b>Settings</b>: generated from the schema</sub>
</td>
</tr>
<tr>
<td align="center">
<img src="https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/assets/screenshots/themes-dark.webp" alt="Themes page, dark">
<br><sub><b>Themes</b>: hand-made, or generated from your wallpaper</sub>
</td>
<td align="center">
<img src="https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/assets/screenshots/themes-light.webp" alt="Themes page, light">
<br><sub><b>Light mode</b>: one toggle switches the pair</sub>
</td>
</tr>
<tr>
<td align="center">
<img src="https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/assets/screenshots/launcher-apps.webp" alt="Launcher">
<br><sub><b>Launcher</b>: apps, windows, math, web and commands</sub>
</td>
<td align="center">
<img src="https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/assets/screenshots/workspace-overlay.webp" alt="Workspace overview">
<br><sub><b>Workspace overview</b>: live previews, drag to move</sub>
</td>
</tr>
</table>

## 🚀 Quick start

> [!NOTE]
> **axiom 1.0 is out**, the first stable release. Configs from earlier versions are migrated automatically.

### Requirements: that's it

The installer below sets these up for you on Arch.

| | |
| --- | --- |
| 🪟 **[Hyprland](https://hypr.land)** 0.55+ | with its Lua config (`hyprland.lua`) |
| 🐚 **[Quickshell](https://quickshell.org)** 0.3.1+ | the `qs` binary |
| 🔤 **[Material Symbols](https://fonts.google.com/icons)** | the icon font (`ttf-material-symbols-variable`); any font works for text |
| 🧰 **`jq`**, **`python3`** | nothing else |

<details>
<summary><b>Optional extras</b>: each one only turns on the feature that uses it</summary>

- `awww`: wallpapers, with transitions
- ImageMagick: theme generation (its Python packages install themselves into a venv)
- NetworkManager: network widget and Wi-Fi menu
- `pacman-contrib`, plus `paru` or `yay`: update checks
- `tailscale`: Tailscale widget
- `grim`, `slurp`, `wl-copy`: screenshots
- `curl`, and `secret-tool` (libsecret) for keys in your keyring: AI chat
- `qalc`: launcher calculator
- `hyprlock` and `hypridle`: hyprlock mode and locking when idle
- The apps you want themed, plus `qt5ct`/`qt6ct` and `adw-gtk-theme`: theme integrations

</details>

### Install

On Arch Linux:

```bash
curl -fsSL https://raw.githubusercontent.com/axiom-dotfiles/axiom/main/install.sh | bash
```

It installs everything from the official repositories. It asks about each optional extra, clones the latest release, and asks before adding the line that starts axiom to your `hyprland.lua`.

By hand, or on another distribution: install the requirements, then

```bash
git clone https://github.com/axiom-dotfiles/axiom.git ~/.config/quickshell/axiom
```

and add the one line your Hyprland config (`hyprland.lua`) needs:

```lua
hl.on("hyprland.start", function() hl.exec_cmd("qs -c axiom") end)
```

Then press <kbd>Super</kbd> + <kbd>Tab</kbd> to open the overlay, and set everything up from the **Settings**, **Themes**, **Bar editor** and **Overlay editor** pages.

> [!TIP]
> By default axiom applies its keybinds and required settings at runtime and writes no files. Any key your config already uses is skipped. **Settings → Desktop → Hyprland** can switch that to a file your `hyprland.lua` includes, or to a `hyprland.lua` that axiom manages.

<details>
<summary><b>Updating</b></summary>

axiom updates itself from its release tags. By default it notifies you when a release is out, and the notification opens **Settings → Updates**, where one click installs it. That page can also switch to updating automatically, or turn checks off. Your settings live in `config/user/config.json`, which git ignores.

axiom won't update a clone with local changes. Update one by hand, saving the changes first:

```bash
git commit -am "local changes"
git pull --rebase origin main
# resolve any conflicts (lazygit makes this painless)
```

</details>

<details>
<summary><b>Uninstalling</b></summary>

```bash
rm -rf ~/.config/quickshell/axiom
rm -rf ~/.local/state/axiom   # generated hyprlock config, chat keys and conversations
```

Then remove the `qs -c axiom` line (marked `-- axiom`) from your `hyprland.lua`. If you'd switched axiom to managing `hyprland.lua`, your original is in `~/.config/hypr/user/00-previous.lua`.

</details>

<details>
<summary><b>Troubleshooting</b></summary>

- **Nothing shows up:** run `~/.config/quickshell/axiom/scripts/log.sh` to see the shell's warnings and errors.
- **Settings won't save:** `config.json` is invalid. The log names the problem. Fix the file, or restore a saved config.
- **Icons show as words** (`wifi`, `battery_full`): the icon font is missing. Install `ttf-material-symbols-variable` and restart the shell.

Found a bug? [Open an issue](https://github.com/axiom-dotfiles/axiom/issues).

</details>

See the [axiom README](https://github.com/axiom-dotfiles/axiom#readme) for the full feature list and the configuration reference.

## 🗺️ Roadmap

- [x] All planned core features
- [x] Big cleanup: config safety, secrets, per-monitor surfaces, unified content and polling
- [x] Install script
- [x] v1.0, the first stable release
- [ ] Onboarding and a setup wizard
- [ ] Clipboard manager
- [ ] More translations
- [ ] Collaboration: CI, issue and PR templates, PR-only changes

## 🤝 Contributing

> [!NOTE]
> Pull requests aren't open yet, and PRs on GitHub will be closed. Issues are very welcome.
> If you want to help (much appreciated), get in touch on Matrix and we can work out how.

Once contributions open:

1. Fork [axiom](https://github.com/axiom-dotfiles/axiom)
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes
4. Push the branch and open a pull request

axiom's `CONTRIBUTING.md` covers its layout and conventions.

## 💬 Support

- **Contact:** @travmonkey:matrix.batk.me
- **Space:** @axiom-dotfiles:matrix.batk.me (not ready yet; moderators wanted)

## 🙏 Acknowledgments

[Hyprland](https://hypr.land/) · [Quickshell](https://quickshell.org/) · [illogical-impulse](https://github.com/end-4/dots-hyprland) · [caelestia-dots](https://github.com/caelestia-dots) · [JaKooLit](https://github.com/JaKooLit/Hyprland-Dots)

The full list, with the fonts, tools and themes axiom builds on, is in the [axiom README](https://github.com/axiom-dotfiles/axiom#-acknowledgments).

## 📄 License

MIT. See [LICENSE](LICENSE).

---

<div align="center">

⭐ **If axiom makes your desktop better, a star helps others find it.**

</div>
