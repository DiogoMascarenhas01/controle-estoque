# Inventory Management

A Python/Tkinter desktop application for managing products, stock movements, users, inventories, and reports.

## Requirements

- Windows 10 or 11
- Python 3.14
- A local MongoDB server available at `mongodb://localhost:27017/`

## Installation

```bash
py -3.14 -m pip install -r requirements.txt
```

Start the MongoDB service, then run:

```bash
py -3.14 inventory_management.py
```

The application uses the existing `ControleDeEstoque` database. Its Portuguese collection names, field names, and persisted movement values are intentionally retained for compatibility with existing data. The interface displays movement types as `INBOUND` and `OUTBOUND`.

## Visual Assets

Keep these files alongside the main Python file:

- `background.png`
- `logo.png`
- `icon.png`

## Security

This version was designed for local use. Before making it available over a network or to multiple users, review account management: the current code stores a plaintext password field in MongoDB for administrative display in addition to the hash used for authentication. Do not use real or reused credentials until this behavior is removed.

## Untracked Files

PyInstaller artifacts, executables, reports, inventories, caches, virtual environments, and local data are excluded by `.gitignore`.
