# Lilium Mobile

A desktop environment for tablets and phones, built on the
[Solium](https://github.com/Lilium-Linux/solium) Wayland compositor. It is
developed on a Surface Pro 7 running Fedora.

**Early preview.** Nothing here is packaged yet: today you put the parts
together by hand, as below.

Community: [Solium on Discord](https://discord.gg/ATQNfHHvFa).

## The parts

| Repository | What it is |
|---|---|
| [solium](https://github.com/Lilium-Linux/solium) | The compositor. It draws the windows and gives the shell its data and its scripting API. |
| [lilium-mobile-shell](https://github.com/Lilium-Linux/lilium-mobile-shell) | The shell: home screen, gestures, Recents, Control Center and lock, written as a Solium configuration (Lua, QML, effects). |
| [lilium-apps](https://github.com/Lilium-Linux/lilium-apps) | The environment's own applications. |
| lilium-mobile (this one) | What makes the parts one environment: installing, packaging and the setup after installation. |

## Putting it together today

1. **Solium**, built from its `stage` branch; its README says how.
2. **The shell:** clone lilium-mobile-shell and run its `install.sh`, which
   makes it your Solium configuration.
3. **Start Solium** from a text console with `solium --tty`.

## License

GPL-3.0-only (`LICENSE`), as Solium and the shell are.
