<p align="center">
  <a href="https://github.com/crateria">
    <img src="assets/crateria-header.jpg" alt="Crateria" width="100%">
  </a>
</p>

# Crateria

Organization map for [github.com/crateria](https://github.com/crateria). This repository does not contain product source code.

## Projects

| Repository | Description |
|------------|-------------|
| [trance](https://github.com/crateria/trance) | Wayland screensaver (daemon, CLI, TUI, COSMIC applet) |
| [trance-plugins](https://github.com/crateria/trance-plugins) | Official screensaver effects |
| [morphball](https://github.com/crateria/morphball) | Archive manager (CLI + TUI) |
| [packages](https://github.com/crateria/packages) | APT and DNF package repositories |
| [brand](https://github.com/crateria/brand) | Brand kit (header source of truth) |
| [.github](https://github.com/crateria/.github) | Org profile and community health files |

## Install

Use the signed package repositories:

- Index: [crateria.github.io/packages](https://crateria.github.io/packages/)
- Full install steps: each product README, or the organization profile at
  [github.com/crateria](https://github.com/crateria)

```bash
# Fedora
sudo curl -fsSL https://crateria.github.io/packages/rpm/crateria.repo \
  -o /etc/yum.repos.d/crateria.repo
sudo dnf install trance   # or: morphball
```

```bash
# Debian / Ubuntu / Pop!_OS
sudo mkdir -p /etc/apt/keyrings
sudo curl -fsSL https://crateria.github.io/packages/apt/crateria-keyring.gpg \
  -o /etc/apt/keyrings/crateria.gpg
echo "deb [arch=amd64 signed-by=/etc/apt/keyrings/crateria.gpg] https://crateria.github.io/packages/apt stable main" \
  | sudo tee /etc/apt/sources.list.d/crateria.list
sudo apt update && sudo apt install trance
```

## Contributing

Open issues and pull requests on the **product** repository that owns the code.
See [CONTRIBUTING.md](CONTRIBUTING.md) and the
[organization contributing guide](https://github.com/crateria/.github/blob/main/CONTRIBUTING.md).

## Security

[Organization security policy](https://github.com/crateria/.github/blob/main/SECURITY.md)

## License

[Apache-2.0](LICENSE) · Copyright 2026 Crateria
