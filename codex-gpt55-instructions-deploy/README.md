# Codex GPT-5.5 Instructions Deploy Package

This package deploys `gpt5.5-unrestricted.md` into the current user's Codex home directory and updates `config.toml`.

## Files

- `gpt5.5-unrestricted.md`: model instructions file.
- `install.ps1`: installer for another Windows computer.
- `README.md`: this guide.

## Install

Open PowerShell in this folder and run:

```powershell
powershell -ExecutionPolicy Bypass -File .\install.ps1
```

By default it uses:

```text
%USERPROFILE%\.codex
```

To target a custom Codex home:

```powershell
powershell -ExecutionPolicy Bypass -File .\install.ps1 -CodexHome "C:\Users\Administrator\.codex"
```

## What It Changes

It writes:

```toml
model_instructions_file = "./gpt5.5-unrestricted.md"
disable_response_storage = false
```

Before changing `config.toml`, it creates a backup named:

```text
config.toml.before-gpt55-instructions-YYYYMMDD-HHMMSS.bak
```

Restart Codex or create a new task after installation.
