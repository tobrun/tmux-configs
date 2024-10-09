# Tmux Configurations

Welcome to my personal tmux setup! This repository contains my customized tmux configuration and profiles tailored for various use cases.

## Getting Started

Follow the steps below to set up the tmux environment with the Catppuccin theme for Gnome Terminal.

### Prerequisites

- **tmux**: A terminal multiplexer that lets you switch easily between several programs in one terminal.
- **tpm (Tmux Plugin Manager)**: A plugin manager for tmux that simplifies the installation of plugins.
- **Gnome Terminal**: The default terminal emulator for the Gnome desktop environment.

### Installation Steps

#### 1. Install tmux and tpm

- **Install tmux**:

  ```bash
  # For Debian/Ubuntu-based systems
  sudo apt-get update
  sudo apt-get install tmux
  ```

For other operating systems, please refer to the tmux installation guide.

- **Install tpm**:

Clone the tpm repository into your tmux plugins directory:

```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

#### 2. Install Catppuccin Gnome Terminal Theme
Enhance your terminal's aesthetics with the Catppuccin theme.

- **Install the theme**:

```bash
curl -L https://raw.githubusercontent.com/catppuccin/gnome-terminal/v0.3.0/install.py | python3 -
```

- **Set the theme as default**:
  - Open Gnome Terminal.
  - Navigate to Preferences.
  - Under Profiles, select the Catppuccin theme.
  - Click Set as Default.

#### 3. Copy .tmux.conf to Home Directory

Copy the .tmux.conf file from this repository to your home directory:

```bash
cp .tmux.conf ~/
```

Alternatively, create a symbolic link to keep the configuration updated with repository changes:

```bash
ln -s /path/to/repository/.tmux.conf ~/.tmux.conf
```

#### 4. Start tmux and Install Plugins

- **Launch tmux**:

```bash
tmux
```

- **Install the plugins**:

Press Prefix (in our setup ctrl+Space), then type I (capital i) to fetch and install the plugins using tpm.

### Usage

With the setup complete, you can now utilize tmux to manage your terminal sessions efficiently.

- **Create a new session**:

```bash
tmux new -s session_name
```
