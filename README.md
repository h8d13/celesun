# CeleSun -  ΦLO-TIME

CeleSun is a 24h clock based on a simple compass (an idea of my dad actually).

We break it down into 15° equal parts (Also 22.5 to be fancy) and work from there.

Built with GTK for a modern, native Linux experience. 

> Clocks are kinda stupid by design, using some neat Python libs we can maybe make a good one? 

---

Uses latitude, longitude and timezone to create GUI. (Defaults to Europe/Paris)

## Installation

### Arch Linux

```bash
# Install system dependencies
sudo pacman -S gtk4 libadwaita python-gobject python-cairo

# Create virtual environment with system packages
python3 -m venv venv --system-site-packages

# Install Python dependencies
./venv/bin/pip install suntime pytz

# Run the application
./venv/bin/python celesun_gtk.py
```

### Ubuntu/Debian

```bash
# Install system dependencies
sudo apt-get install python3-gi python3-gi-cairo gir1.2-gtk-4.0 gir1.2-adw-1 python3-venv

# Create virtual environment with system packages
python3 -m venv venv --system-site-packages

# Install Python dependencies
./venv/bin/pip install suntime pytz

# Run the application
./venv/bin/python celesun_gtk.py
```

### Fedora

```bash
# Install system dependencies
sudo dnf install gtk4 libadwaita python3-gobject python3-cairo

# Create virtual environment with system packages
python3 -m venv venv --system-site-packages

# Install Python dependencies
./venv/bin/pip install suntime pytz

# Run the application
./venv/bin/python celesun_gtk.py
```

---

## Configuration

Settings are automatically saved to `~/.config/celesun/config.json` and include:

---
