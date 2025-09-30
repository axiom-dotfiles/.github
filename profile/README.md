# <div align="center">Axiom Dotfiles</div>

<!-- Badges -->
<div align="center">

[![Organization Followers](https://img.shields.io/github/followers/axiom-dotfiles?style=for-the-badge&logoColor=ebdbb2&labelColor=282828&label=Follow&color=458588)](https://github.com/axiom-dotfiles)
[![Stars](https://img.shields.io/github/stars/axiom-dotfiles/axiom?style=for-the-badge&logoColor=ebdbb2&labelColor=282828&color=d79921)](https://github.com/axiom-dotfiles/axiom)
[![Latest Commit](https://img.shields.io/github/last-commit/axiom-dotfiles/axiom?style=for-the-badge&logoColor=ebdbb2&labelColor=282828&color=98971a)](https://github.com/axiom-dotfiles)

</div>

<!-- Video Demo -->
<!-- [![Demo Video](https://img.youtube.com/vi/YOUR_VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID) -->

## Info

[Axiom Dotfiles](https://github.com/axiom-dotfiles) is my personal collection of dotfiles and configurations for Hyprland and related tools, designed to create a cohesive, feature-packed, and visually appealing desktop environment.

### Features

- **Grid-Based Workspaces**: Completely new way to manage workspaces using a grid system
- **Color Generation**: Generate color schemes based on your wallpaper
- **Pinnable AI Chat**: Pinnable Menu panel with built-in AI chat functionality
- **Application Based OSD**: Set multiple applications for the OSD

#### Planned

- [ ] Onboarding + Setup Wizard
- [ ] Clipboard manager
- [ ] Dice roller???
- [ ] First stable release -> Moving from chaos in git history to merged PRs only
- [ ] AUR Package
- [ ] Improved Modularity, Docuemntation, and Configuration

## Structure

This organization contains modular repositories for different components:

- Widgets: **[axiom](https://github.com/axiom-dotfiles/axiom)**
- Hypr Config: **[hypr](https://github.com/axiom-dotfiles/hypr)**
<!-- - **[repo-name]**: [Component description] -->
<!-- - **[repo-name]**: [Component description] -->

# Installation

> [!NOTE]
> Installations are not officially supported yet, and the setup may be quite obnoxious.
> Please be patient as development is ongoing. You likely can get it working with some effort though :)
> Keep in mind breaking changes to `config.json` will certainly occur until the first stable release.
> The config schema will also not be updated until the first stable release.

## Docker

TODO: Add Docker setup and instructions.
> [!Note]
> Docker setup is not ready yet.
> Should run daemonless (e.g. podman)
> Currently planning to build quickshell in CI and push to GHCR

## Native
### Automated (not ready yet)

TODO: Add installation script and AUR package

### Manual

#### Dependencies

TODO: Find all dependencies

**Required:**
- Dependency 1 ([version/range])

**Optional:**
- Optional Dependency 1: ([version/range])([purpose])

```bash
# Good luck. This is not really ready for public use yet :)
git clone https://github.com/axiom-dotfiles/axiom.git ~/.config/quickshell/axiom
git clone https://github.com/axiom-dotfiles/hypr.git ~/.config/hypr
# ... debug
```

## Configuration

Configuration is available via `config/config.json`

## Updating

```bash
# No managed installation available yet :(
cd ~/.config/quickshell/axiom
git pull origin main
cd ~/.config/hypr
git pull origin main
```

## Uninstalling

```bash
# Remove configuration directories
```

## Troubleshooting

TODO: Add common issues and solutions here.

## Contributing

> [!Note]
> Contributions are not ready yet, and pull requests will be closed. Feel free to open issues though!

> [!Note]
> If you really want to help contribute before the first stable release (totally appreciated), please reach out to me on Matrix (@travmonkey:matrix.org)
> and we can discuss collaboration options and methods.

For when contributions are ready:
Contributions are welcome! Please feel free to submit a Pull Request to any of the repositories in this organization. (see above, not ready yet, PR's on github will be closed)

1. Fork the relevant repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE)

## Acknowledgments / Inspirations / References

- [hyprland](https://hypr.land/)
- [quickshell](https://quickshell.org/)
- [End-4](https://github.com/end-4/dots-hyprland)
- [caelestia-dots](https://github.com/caelestia-dots)
- [JaKooLit](https://github.com/JaKooLit/Hyprland-Dots)

## Support

- **Contact**: @travmonkey:matrix.org
- **Space**: @axiom-dotfiles:matrix.org (not ready yet) (potentially looking for moderators)

---

⭐ If you find this useful, please consider starring the repositories!

> [!Note]
> Trying to donate? Sorry, I don't accept donations. If you want to support the project, please consider contributing code or spreading the word!
