# Watcher42

**Fast Pi Node Watcher for Windows**

Watcher42 is a lightweight, read-only monitoring tool for Pi Node.  
It runs as a PowerShell script on the Windows host and reads information from Docker, the Pi Node container and the local Horizon API.

## What it shows

- Docker and Pi Node container status
- Docker image
- Core and Protocol version
- Consensus state and blockchain sync
- Local and network block
- Blocks behind
- Horizon API status
- Incoming and outgoing connections
- Pi Node availability
- Refresh status

## Availability history

Watcher42 can keep a local `availability.json` history.

- One availability value per day
- Newest entries stored first
- Existing history is preserved
- Availability monitoring can be disabled in `config.json`

`IMPORT_HISTORY.bat` can import and merge an `availability.json` from a previous Watcher42 version. Existing data is backed up before importing.

## Requirements

- Windows 10 or Windows 11
- Docker Desktop
- Pi Node / Pi Desktop
- Windows PowerShell

## Installation

1. Download the latest Watcher42 ZIP from **Releases**.
2. Extract the ZIP.
3. Run `START_WATCHER42.bat`.
4. Press `CTRL+C` to stop Watcher42.

No installation is required.

## Configuration

Basic settings can be changed in `config.json`, including refresh intervals, container name and availability monitoring.

## Read-only

Watcher42 is designed as a monitoring tool only.

It does **not** restart Docker or Pi Node, change Pi Node settings, modify Docker configuration, or modify blockchain data.

## Current version

**Watcher42 v1.1**

Tested on Windows 10 and Windows 11.

---

Watcher42 is an independent community tool and is not an official Pi Network application.
