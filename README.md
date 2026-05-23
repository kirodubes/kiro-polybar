<p align="center">
  <img src="kiro.jpg" alt="Kiro" width="220" />
</p>

# edu-polybar

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
sudo pacman -S edu-polybar-git
```

You'll also need polybar:

```bash
sudo pacman -S polybar
```

### Manual

```bash
git clone https://github.com/erikdubois/edu-polybar.git
cd edu-polybar
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

## License

See [LICENSE](./LICENSE).
