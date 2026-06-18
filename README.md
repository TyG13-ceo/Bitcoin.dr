# Core‑TyG Node Optimization

Core‑TyG is a modular toolkit for optimizing, automating, and maintaining Bitcoin Core nodes inside Termux on Android. It includes prune‑mode repair, RPC stabilization, PSBT/UTXO tools, and ASIC miner configuration syncing.

## Features
- Prune‑mode repair: detects and fixes prune mismatches that prevent node startup.
- RPC stabilization: reduces timeout errors and improves command reliability.
- ASIC sync automation: keeps miners aligned with your pool and payout address.
- PSBT and UTXO tools: build, sign, and broadcast transactions using reusable modules.
- Termux‑optimized scripts: lightweight, deterministic shell modules for Android‑based node control.

## Requirements
- Android 10 or higher
- Termux (latest version)
- Bitcoin Core v26 or higher
- Python 3.11 or higher (optional modules)
- Git

## Installation
pkg install git
git clone https://github.com/TyG13-ceo/Bitcoin.dr.git
cd Bitcoin.dr
bash setup.sh

## Configuration
Edit bitcoin.conf and .env to match your node setup.

Your payout address:
3Mm9vjGN4oHEbJdBWpVMvxzzcVaPyHymyk

## Usage
Run the main optimization suite:
bash core-tyg.sh

Run pruning and RPC diagnostics:
bash auto-prune.sh && bash rpc-check.sh

Run UTXO and PSBT tools:
bash psbt-tool.sh

## Directory Structure
.github/workflows  - GitHub Actions CI/CD automation
scripts/           - Termux-ready shell modules
config/            - Node and miner configuration files
docs/              - Technical documentation

## Contributing
Pull requests are welcome. For major changes, open an issue to discuss your proposal first.

## License
MIT License — free to modify and redistribute.
