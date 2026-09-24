# <div align="center">Axiom Dotfiles</div>

<!-- Badges -->
<div align="center">

[![Organization Followers](https://img.shields.io/github/followers/axiom-dotfiles?style=for-the-badge&logoColor=ebdbb2&labelColor=282828&label=Follow&color=458588)](https://github.com/axiom-dotfiles)
[![Stars](https://img.shields.io/github/stars/axiom-dotfiles/axiom?style=for-the-badge&logoColor=ebdbb2&labelColor=282828&color=d79921)](https://github.com/axiom-dotfiles/axiom)
[![Latest Commit](https://img.shields.io/github/last-commit/axiom-dotfiles/axiom?style=for-the-badge&logoColor=ebdbb2&labelColor=282828&color=98971a)](https://github.com/axiom-dotfiles/axiom)

</div>

https://github.com/user-attachments/assets/a53f62e0-e2bc-4834-a05f-92b6cb115c35

A complete, themeable Hyprland desktop, built on [Quickshell](https://quickshell.org). It covers the bar, the overlay, notifications, the lockscreen, the launcher and the power menu. You configure it from inside the shell, and it takes its colors from your wallpaper.

## Highlights

- **Configured from the desktop.** The settings page is generated from the config schema. The bar and the overlay each have a live editor, and every change hot-reloads with no restart. A broken config never replaces the running one.
- **Bars your way.** Any number of bars, on any monitor and any edge: solid, transparent, or floating pills that merge into the screen border. 21 widget types, with popouts that grow out of the bar.
- **The overlay.** Full-screen pages of cards that you lay out yourself, from 23 modules: media, mixer, system graphs, processes, weather, calendar, notes, quick toggles, AI chat and more. Each module adapts to the shape of its slot.
- **Grid-based workspaces.** A 5×5 workspace grid on each monitor, with a bar widget, a workspace map and a workspace overlay to move around it.
- **Colors from your wallpaper.** pywal backends pick the candidate colors, then the palette is built in OKLCH to match the contrast of the hand-made themes. There are dark/light pairs of Catppuccin, Gruvbox, Solarized and Tokyo Night, plus Submarine Sonar.
- **One theme everywhere.** kitty, cava, k9s, Neovim and hyprlock follow the active theme.
- **Per-app OSD.** The volume OSD follows the apps you choose, not only the master volume.
- **AI chat.** Gemini, OpenAI, Anthropic or offline, in an overlay card. API keys are kept out of the config.
- **Your choice of lockscreen.** The built-in Wayland session lock (PAM), a themed hyprlock config that axiom generates, or bring your own.
- **Multi-monitor and translated.** Per-monitor wallpapers and bars. English and Japanese, with more added as a single JSON file each.

## Repositories

| Repository | What it is | Installs to |
| --- | --- | --- |
| **[axiom](https://github.com/axiom-dotfiles/axiom)** | The Quickshell desktop shell: bar, overlay, notifications, lockscreen, launcher, OSD | `~/.config/quickshell/axiom` |
| **[hypr](https://github.com/axiom-dotfiles/hypr)** | The Hyprland config, with keybinds for axiom and a hypridle setup | `~/.config/hypr` |
| **[install](https://github.com/axiom-dotfiles/install)** | Installation pieces, currently a greetd + ReGreet login setup | `/etc/greetd` |

See the [axiom README](https://github.com/axiom-dotfiles/axiom#readme) for the full list of features and the configuration reference.

## Installation

> [!NOTE]
> There's no official installer yet, so setup is manual. Expect some rough edges.
> Until the first stable release, `config.json` may still change between versions. Old configs are migrated automatically.

### Dependencies

**Required:** Hyprland, [Quickshell](https://quickshell.org) 0.3.1 or newer, a Nerd Font (`Symbols Nerd Font`), `jq`, `python3`.

**Optional:**
- `awww`: wallpapers
- ImageMagick: theme generation
- NetworkManager: network widget
- `pacman-contrib`, plus `paru` or `yay`: update checks
- `tailscale`
- `grim`, `slurp`, `wl-copy`: screenshots
- `hyprlock` and `hypridle`
- `kitty`, `cava`, `k9s`, `nvim`: theme integrations

### Manual

```bash
git clone https://github.com/axiom-dotfiles/axiom.git ~/.config/quickshell/axiom
git clone https://github.com/axiom-dotfiles/hypr.git ~/.config/hypr
```

The hypr config starts the shell for you. If you use your own Hyprland config instead, add:

```ini
exec-once = QML_XHR_ALLOW_FILE_READ=1 qs -c axiom
bind = SUPER, TAB, exec, qs -c axiom ipc call overlay toggle
```

Then open the overlay and set things up from the **Settings**, **Themes**, **Bar editor** and **Overlay editor** pages.

### Automated

An install script and an AUR package are planned.

## Updating

There's no managed update yet. If you haven't changed the source, `git pull` in each repository is enough. Your settings live in `config/user/config.json`, which git ignores.

If you have local changes, save them first:

```bash
git commit -am "local changes"
git pull --rebase origin main
# resolve any conflicts (lazygit makes this painless)
```

## Uninstalling

```bash
rm -rf ~/.config/quickshell/axiom ~/.config/hypr
rm -rf ~/.local/state/axiom   # generated hyprlock config and chat API keys
```

## Troubleshooting

- **Nothing shows up:** run `~/.config/quickshell/axiom/scripts/log.sh` to see the shell's warnings and errors.
- **Settings won't save:** `config.json` is invalid. The log names the problem. Fix the file, or restore a saved config.
- **Missing icons:** install a Nerd Font that provides `Symbols Nerd Font`.

Found a bug? [Open an issue](https://github.com/axiom-dotfiles/axiom/issues).

## Roadmap to v1.0

- [x] All planned core features
- [x] Big cleanup: config safety, secrets, per-monitor surfaces, unified content and polling
- [ ] Onboarding and a setup wizard
- [ ] Clipboard manager
- [ ] Install script and management
- [ ] Collaboration: CI, issue and PR templates, PR-only changes after the first release

## Contributing

> [!NOTE]
> Pull requests aren't open yet, and PRs on GitHub will be closed. Issues are very welcome.
> If you want to help before the first stable release (much appreciated), get in touch on Matrix and we can work out how.

Once contributions open:

1. Fork the relevant repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes
4. Push the branch and open a pull request

Each repository's `CONTRIBUTING.md` covers its layout and conventions.

## License

MIT. See [LICENSE](LICENSE).

## Acknowledgments

- [Hyprland](https://hypr.land/)
- [Quickshell](https://quickshell.org/)
- [illogical-impulse](https://github.com/end-4/dots-hyprland)
- [caelestia-dots](https://github.com/caelestia-dots)
- [JaKooLit](https://github.com/JaKooLit/Hyprland-Dots)

## Support

- **Contact**: @travmonkey:matrix.batk.me
- **Space**: @axiom-dotfiles:matrix.batk.me (not ready yet; moderators wanted)

---

⭐ If you find this useful, please consider starring the repositories!

> [!NOTE]
> Interested in the keyboard? Check out my keyboard project: [travyboard](https://github.com/travishepworth/travyboard-mirror)

> [!NOTE]
> Interested in Kubernetes? Check out [Klusteroth](https://code.batk.me/Kubernetes) and my [template-application](https://code.batk.me/Kubernetes/template-application).

> [!NOTE]
> I don't accept donations. If you want to support the project, contribute code or spread the word!
