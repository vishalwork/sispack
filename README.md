# Sispack 🗂️
> Built to help users easily track and analyze installed package sizes on their system.

![Shell](https://img.shields.io/badge/Shell-Bash-green) ![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS-blue) ![License](https://img.shields.io/badge/License-MIT-yellow)

---

## Supported Platforms

| Platform | Package Manager |
|----------|----------------|
| Debian / Ubuntu | `dpkg` |
| Fedora / RHEL / CentOS | `rpm` |
| Arch Linux | `pacman` |
| macOS | `Homebrew` + `/Applications` |

---

## Installation

### Debian / Ubuntu
```bash
git clone https://github.com/vishalwork/sispack.git
cd sispack
chmod +x sispack
mv sispack ~/.local/bin/
```
> Or download `.deb` from releases:
> ```bash
> sudo dpkg -i sispack.deb
> ```

### macOS
```bash
git clone https://github.com/vishalwork/sispack.git
cd sispack
chmod +x sispack
sudo mv sispack /usr/local/bin/
```
> **Note:** Homebrew must be installed for package tracking.
> Install Homebrew: https://brew.sh

### Arch Linux
```bash
git clone https://github.com/vishalwork/sispack.git
cd sispack
chmod +x sispack
mv sispack ~/.local/bin/
# ~/.local/bin PATH mein nahi hai toh:
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc && source ~/.bashrc
```

### RPM (Fedora / RHEL / CentOS)
```bash
git clone https://github.com/vishalwork/sispack.git
cd sispack
chmod +x sispack
mv sispack ~/.local/bin/
```

---

## Usage
```bash
sispack          # List all packages by size
sispack -r       # Reverse order
sispack -f name  # Search specific package
sispack -a       # Author info
sispack -h       # Help
sispack -v       # Version
```

---

## Author

Made with ❤️ by **Vishal Kumar** — [@vishalwork](https://github.com/vishalwork)
Originally forked from [@vlc-ranchi](https://github.com/vlc-ranchi)
