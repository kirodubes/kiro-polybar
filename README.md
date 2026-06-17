<p align="center">
  <img src="kiro.jpg" alt="Kiro" width="220" />
</p>

# kiro-polybar

Educational / tutorial repository for [polybar](https://github.com/polybar/polybar), a fast and easy-to-use status bar. Part of the `~/EDU/` learning series — a ready-to-use polybar config dropped on top of a fresh Arch / Kiro install.

## What's in this repo

- `etc/skel/.config/polybar/config.ini` — the main polybar configuration.
- `etc/skel/.config/polybar/launch.sh` — launcher script that starts polybar against the right monitor(s).
- `etc/skel/.config/polybar/scripts/` — helper scripts referenced by `config.ini` (network info, volume, weather, etc.).
- `setup.sh`, `up.sh` — standard EDU bash scaffold.

## Installation

### From `nemesis_repo` (recommended)

```ini
[nemesis_repo]
SigLevel = Never
Server = https://erikdubois.github.io/$repo/$arch
```

```bash
sudo pacman -Syu
sudo pacman -S kiro-polybar
```

You'll also need polybar:

```bash
sudo pacman -S polybar
```

### Manual

```bash
git clone https://github.com/kirodubes/kiro-polybar.git
cd kiro-polybar
sudo cp -r etc/skel/. /etc/skel/
```

Existing users can pull the config into their own home:

```bash
cp -rT /etc/skel ~/
```

## Usage

Start polybar from your WM's autostart (or by hand) by invoking the launcher script:

```bash
~/.config/polybar/launch.sh
```

Edit `~/.config/polybar/config.ini` to swap modules in / out, change colours, or rebind which bar appears on which monitor.

## Websites

Information : https://erikdubois.be

## Social Media

Youtube : https://www.youtube.com/erikdubois

<!-- KIRO-FUNDING-FOOTER:START — managed by Kiro-HQ/cascade-readme-footer.sh -->
## Help fund Kiro

Everything I build here stays free and open — always. If Kiro or any of these
tools have ever saved you time or taught you something, a small monthly
contribution helps keep the work going. Donations target break-even, nothing
more — the core always stays free for everyone.

- GitHub Sponsors: https://github.com/sponsors/erikdubois
- Patreon: https://www.patreon.com/c/kiroproject
- YouTube memberships: https://www.youtube.com/@ErikDubois/join
- Ko-fi: https://ko-fi.com/erikdubois
- PayPal: https://www.paypal.me/erikdubois
<!-- KIRO-FUNDING-FOOTER:END -->

## License

See [LICENSE](./LICENSE).
