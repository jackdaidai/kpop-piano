[English](README.md) | [简体中文](README.zh-CN.md)

# KPop Demon Hunters Piano 🎹

A single-file browser piano game for kids, built around songs from *KPop Demon Hunters*.

## Overview

Open `index.html` and play — no build step, no server, no install. A 3D piano keyboard (rendered with three.js) fills the screen; falling note bars tell you which key to hit next, like a rhythm game. It's designed for a child who can't read music yet: every note is called out by name so they always know what to press.

## Features

- **8 songs** from *KPop Demon Hunters* (Golden, Soda Pop, How It's Done, Your Idol, Takedown, Free, What It Sounds Like, and a Takedown · TWICE version), plus a **Free Play** mode
- **Two play modes**
  - 🌱 Learn mode — a side card shows the next note name and offers an 8-note audio demo, so the player never has to guess
  - ⚡ Rhythm mode — notes scroll down and must be hit in time, with an adjustable fall speed slider
- **Scoring** — hit judgement (with pop animation), combo counter, a 3-star rating and score summary on song completion
- **Two input methods** — click/tap the 3D keys, or play from the computer keyboard (mapped across two octaves starting at C4)
- Fully self-contained: a single `index.html` file, in Chinese UI

## Tech Stack

- Vanilla JavaScript, no build tooling
- [three.js](https://threejs.org/) r128 (loaded from CDN) for the 3D piano rendering
- Web Audio API for synthesized piano tones

## Quick Start

No install needed — just open the file in a browser:

```bash
# from the repo root
open index.html        # macOS
start index.html        # Windows
```

Or serve it locally (useful for some browsers' local-file restrictions):

```bash
npx serve .
```

Then visit the printed local URL.

## Project Structure

```
index.html   # everything — markup, styles, game logic, song data
```
