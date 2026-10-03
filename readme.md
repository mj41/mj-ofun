# Overview

Various [mj41's projects](https://github.com/mj41).

# VS Code Related Projects

## stai-vscode

Toolset and configuration for Visual Studio Code.

git repo: [stai-vscode](https://github.com/mj41/stai-vscode)

### cmd/vscode-bin-manager

VS Code binary manager for downloading, installing, and managing multiple VS Code insiders daily builds.

### cmd/ws-config-gen

VS Code automation and configuration tools.

Generates VS Code separate profiles and Fedora Linux desktop shortcuts:
![stai-fedora-profiles](imgs/stai-fedora-profiles.png)

Each has its own settings, extensions, configurations and title bar color:
![stai-vscode-E](imgs/stai-vscode-E.png)

### stai-vscode-userconf

User configuration templates for VS Code.
```
~/work-stai/stai-vscode-userconf [main L|✔]$ tree
.
├── common
│   ├── app-settings.json.merge.tmpl
│   ├── extensions.txt.merge.tmpl
│   └── user-settings.json.tmpl
├── insiders-B
│   └── stai-all.code-workspace.merge.tmpl
├── insiders-C
│   └── stai-all.code-workspace.merge.tmpl
├── insiders-D
│   └── stai-all.code-workspace.merge.tmpl
├── insiders-E
│   ├── stai-all.code-workspace.merge.tmpl
│   └── user-settings.json.merge.tmpl
└── readme.md
```

git repo: [stai-vscode-userconf](https://github.com/mj41/stai-vscode-userconf)

## stai-copilot

Contains VS Code Copilot configuration files in `.github` directory.

git repo: [stai-copilot](https://github.com/mj41/stai-copilot)

## stai-bins

Binaries and documentation for various tools including aicmd and aiterm.

git repo: [stai-bins](https://github.com/mj41/stai-bins)

## stai-tools

stai-bin tools source code and related utilities.

git repo: [stai-tools](https://github.com/mj41/stai-tools)

# Git Related Projects

## gl-git-links

The `gl:` git-links specification and related tools.

git repo: [gl-git-links](https://github.com/mj41/gl-git-links)

## vscode-gl-git-links

Visual Studio Code extension for `gl:` git link syntax. See `gl-git-links` repo above. Features clickable links, quick fixes, line number support, and more.

git repo: [vscode-gl-git-links](https://github.com/mj41/vscode-gl-git-links)

## gl-exA, gl-exA-src

`gl-exA` is an example repository for `gl-git-links` tools. `gl-exA-src` contains assets to programmatically generate the `gl-exA` git repository including git history.

git repos:
- [gl-exA](https://github.com/mj41/gl-exA)
- [gl-exA-src](https://github.com/mj41/gl-exA-src)

# git-rgen-tool

Tool to programmatically generate git repositories from structured assets.

git repo: [git-rgen-tool](https://github.com/mj41/git-rgen-tool)

## git-wmem

Git based utils to track uncommitted changes in multiple git repositories. Triggered by events, periodically or manually.

git repo: [git-wmem](https://github.com/mj41/git-wmem)

## git-mj-rebase

Git rebase tool.

git repo: [git-mj-rebase](https://github.com/mj41/git-mj-rebase)

## vscode-staiwatch-logger

A VS Code extension that logs workspace and file events to JSONL files for audit and analysis purposes.

git repo: later

## git-wmem-exa1

Automated tools to generate comprehensive HTML documentation of git-wmem state transitions using real git-wmem-commit binaries.

git repo: later

# IPM - Infinite Process Modeling

## ipm-drawio

Utilities for exploring the ipm text format (`.ipmt`) and converting diagrams to and from draw.io.

git repo: soon

## ipm-example-small

Demonstrate distributed logging across multiple Go modules.

git repo: soon

## ipm-fuzzy-match

A tool for matching program log entries to their source code locations using exact literal pattern matching. Takes output from `ipm-golog-refs` (metadata about log calls in source code) and program log output, then correlates log records to specific source code lines using shortest unique substring algorithms.

git repo: soon

## ipm-golog-refs

Analyzes Go source code to extract and catalog logging calls.

git repo: soon

## ipm-ptrace

Advanced ptrace-based filesystem monitoring with race-free file snapshotting for Linux (Fedora 42+).

git repo: soon

## ipm-trace-proc

Integrated `ipm-golog-refs`, `ipm-ptrace` `and ipm-fuzzy-match` tool to trace program execution and correlate log entries, ptrace events and source code lines.

git repo: soon

# home-w42-eu: a local first home platform, with Stackchan robots

A **local first, security and privacy first platform for a home**: Go servers on a small
machine at home, every device (new or old) a light client of them, and loops that AI
helps you write and you approve. The first devices are M5Stack Stackchan robots and a
micro:bit car. All proofs of concept, vibe coded, not reviewed by humans yet.

Public instance of the robot dashboard: [chan.w42.eu](https://chan.w42.eu).

## home-w42-eu

Vision, use cases (the main driver), principles, architecture and the device wire protocol.

git repo: [home-w42-eu](https://github.com/mj41/home-w42-eu)

## home-w42-eu-ideas

Ideas for devices, adapters and loops: old phones, a Roomba, Home Assistant, a private GPS
app, cameras, Wi-Fi presence, calendars, personal captures, local voice.

git repo: [home-w42-eu-ideas](https://github.com/mj41/home-w42-eu-ideas)

## StackChan firmware: Embody Mode

Fork of [m5stack/StackChan](https://github.com/m5stack/StackChan) with the Embody Mode app:
the robot as a light client of a server you choose (camera, microphone, speaker, every
sensor as raw data, commands), switchable between servers and apps. Optional: it drives a
TPBot car over BLE, and servers can automate it. Setup guide:
[SETUP.md](https://github.com/mj41/StackChan/blob/embody-mj41/firmware/main/apps/app_embody_mode/SETUP.md).

git repo: [StackChan, branch embody-mj41](https://github.com/mj41/StackChan/tree/embody-mj41)

## stackchan-server

Relay and dashboard for Stackchan robots in Embody Mode (Go, single binary), and the Go
implementation of the wire protocol. The robot connects out over WebSocket, and a phone
pairs by scanning the QR code on the robot's screen. The phone then gets a live dashboard:
camera, microphone, speaker, head motion, face, LEDs, every sensor, IR, NFC, files.

git repo: [stackchan-server](https://github.com/mj41/stackchan-server)

## stackchan-pet

A Tamagotchi for Stackchan (Go), a second Embody Mode server the robot switches to. Kids
care for the pet on the robot itself (head touches, NFC food cards, menus on the screen) and
on a picture page on a phone. Games, a photo leaderboard, and a parent page with the daily
routine behind a PIN. Czech and English.

git repo: [stackchan-pet](https://github.com/mj41/stackchan-pet)

## sbot

The seed of the home node: a web/API server with a cockpit for a Stackchan and a TPBot car
(camera, joystick, head pad, lights, a sonar safety stop), an event hub (NATS JetStream),
and a controller server for loops.

git repo: [sbot](https://github.com/mj41/sbot)

## tpbot-ble

micro:bit V2 firmware (TinyGo) for the ELECFREAKS TPBot car: a BLE peripheral with raw
sensors and a watchdog, plus a laptop tool and a bridge.

git repo: [tpbot-ble](https://github.com/mj41/tpbot-ble)

## stackchan-mj

Notes, scripts and tools for working on Stackchan with Embody Mode: build and flash, run the
servers in the background, hardware coverage, the trust design.

git repo: [stackchan-mj](https://github.com/mj41/stackchan-mj)

# Others

## minecraft-fedora-installer

Per-user Minecraft launcher installer for Fedora Linux (Go). Downloads the official launcher, installs it into XDG locations, and creates a desktop entry with automatic GPU detection.

git repo: [minecraft-fedora-installer](https://github.com/mj41/minecraft-fedora-installer)

## mj-ofun

This repository.

git repo: [mj-ofun](https://github.com/mj41/mj-ofun)

## profiles-stai

Local directory for stai-vscode generated VS Code profiles.

### opt

Local directory for VS Code insiders binaries and extensions-cache directories.
