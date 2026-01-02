# SHELL_SCRIPTS

> A collection of different scripts that make my life as a Linux user a little easier, because I do not possess a photographic memory :D (darn it)

---

## Available Scripts

### `update_system`
**Complete system maintenance and update script for Linux Mint**

---

## Usage

### Basic System Update
```bash
./update_system
```
Updates all system packages, drivers, and user-installed software.

### System Update + Cache Cleaning
```bash
./update_system -c
```
Same as above, plus cleans:
- Thumbnail cache and temporary files
- Memory caches
- Browser caches and cookies

---

## Features

### System Updates
- **Package Management**: Updates APT packages, distribution upgrades
- **Drivers**: Automatically installs latest drivers via `ubuntu-drivers`
- **Mirror Optimization**: Tests and selects fastest download mirrors
- **Time Sync**: Enables automatic NTP time synchronization

### Software Updates
- **Flatpak**: Updates Flatpak applications and optimizes remotes
- **Snap**: Updates Snap packages
- **Python**: Updates user-installed Python packages via pip3
- **Node.js**: Updates global npm packages
- **Ruby**: Updates user Ruby gems

### Cache Cleaning (with `-c` flag)
- **System Files**: Thumbnails, temp files, trash
- **Memory**: Clears system memory caches
- **Browsers**: Firefox, Chrome, Chromium caches and cookies

### User Experience
- **Colored Output**: 
  - Yellow for "Starting..." messages
  - Green for successful operations
  - Red for failures and missing services
- **Error Handling**: Graceful handling of missing services/tools
- **Progress Feedback**: Clear status updates for each operation

---

## Requirements

- **OS**: Linux Mint (or Ubuntu-based distributions)
- **Privileges**: sudo access for system operations
- **Optional**: Flatpak, Snap, pip3, npm, gem (script handles missing tools)

---

## Output Colors

| Color | Meaning |
|-------|---------|
| **Yellow** | Operation in progress |
| **Green** | Operation successful |
| **Red** | Operation failed or service missing |

---

## Future Scripts

*This repository is designed to be expandable. Future scripts will be documented here with similar detailed usage instructions.*

---

## Quick Reference

| Command | Description |
|---------|-------------|
| `./update_system` | Basic system update |
| `./update_system -c` | Update + deep clean |
| `./update_system -h` | Show usage help |

---

***Tip**: Run with `-c` flag weekly for optimal system performance!*

---

*Last updated: 1/2/2026*
