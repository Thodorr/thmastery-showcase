# THMastery

![Godot](https://img.shields.io/badge/Godot-3.5.3-478CBF?logo=godotengine&logoColor=white)
![GDScript](https://img.shields.io/badge/GDScript-355570?logo=godotengine&logoColor=white)
![Dialogic](https://img.shields.io/badge/Dialogic-1.4.5-6E4BC4)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D6?logo=windows&logoColor=white)
![Status](https://img.shields.io/badge/Status-Playable%20Vertical%20Slice-success)

**A narrative no-combat CRPG set on the THM campus in Gießen.**

![THMastery gameplay preview: skill check and outfits](media/preview.gif)

## Trailer

https://github.com/user-attachments/assets/7b968190-f7be-47ed-b0b0-be96049a4204

## About

**THMastery** is a 2D narrative CRPG inspired by *Disco Elysium*. You play a new student at THM whose studies, conversations and decisions determine which paths through the game are available.

> **Status:** playable vertical slice / prototype

## Features

- Dialogue choices change NPC affinity, later conversations and the ways a task can be solved.
- Active and passive skill checks use one of ten attributes, a D20 roll and situational modifiers. Active checks are chosen by the player; a tooltip shows the success probability, the required roll and the modifiers. Passive checks happen automatically when the character is good enough to notice something.
- Courses follow a Digital Media Systems degree structure and grant skills that open up new options.
- Nerve acts as the game's health system. Stress reduces it; sleep, food and other activities restore it.
- Repeated choices can unlock personality traits with advantages and drawbacks.
- Equipment (27 outfits, 13 hats, face accessories and trinkets) changes the character's appearance and attributes.
- The campus contains NPCs, readable documents, vendors, equipment, consumables and context-sensitive interactions.
- Additional content can be loaded at runtime through a DLC menu.

## Current demo

The current build is a vertical slice around the start of the game. It includes:

- the introduction area, which teaches movement, dialogue, tasks, items and checks;
- the entrance level of Building A10, including the Pastaria, main hall and Mensa;
- a small exterior area around A10 with side content, a vendor and hidden items;
- example tasks with several solutions, including dialogue, item and exploration routes;
- menus for attributes, tasks, inventory, skills, options and the HUD.

The demo covers the beginning of the game. The rest of the campus and the main story are not part of it yet.

## Download

1. Download `THMastery_Windows.zip` from the [latest release](https://github.com/Thodorr/thmastery-showcase/releases/latest).
2. Unzip it and start `THMastery.exe`. No installation is required.

> **Note:** The executable is not code-signed, so Windows SmartScreen may show a warning on first launch. Choose **More info → Run anyway**.

## Controls

THMastery can be played almost entirely with the mouse.

| Input | Action |
| --- | --- |
| Left mouse button | Move, interact, select |
| Right mouse button | Inspect an object or use an inventory item |
| Hold left mouse button | Open the context menu for an object |
| `T` | Open tasks |
| `I` | Open inventory |
| `C` | Open attributes |
| `K` | Open skills |
| `Esc` | Open game menu |
| `Space` | Select the default dialogue option |

## Technology

- **Godot Engine 3.5** with **GDScript**
- **Dialogic 1.4.5**, extended for THMastery's dialogue and skill-check systems (custom choice buttons with check labels, probability tooltips and dice animation)

## Documentation

- **Game Design Document:** [docs/GD-Dokument_THMastery.pdf](docs/GD-Dokument_THMastery.pdf)

## Assets and licences

THMastery uses third-party assets, primarily from LimeZu's *Modern* collections. These assets have their own licence terms and are not automatically covered by a licence for this repository's source code.

Before redistributing the project, please check the terms for all included assets and keep the corresponding credits and licences with the project.
