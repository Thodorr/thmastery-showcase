# THMastery

![Godot](https://img.shields.io/badge/Godot-3.5.3-478CBF?logo=godotengine&logoColor=white)
![GDScript](https://img.shields.io/badge/GDScript-355570?logo=godotengine&logoColor=white)
![Dialogic](https://img.shields.io/badge/Dialogic-1.4.5-6E4BC4)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D6?logo=windows&logoColor=white)
![Status](https://img.shields.io/badge/Status-Playable%20Vertical%20Slice-success)

**A narrative no-combat CRPG set on the THM campus in Gießen.**

![THMastery gameplay preview: skill check and outfits](docs/media/preview.gif)

---

## Trailer

<!-- Drag THMastery_Trailer_1080p.mp4 into the GitHub README editor and replace the line below with the generated link. -->
https://github.com/user-attachments/assets/REPLACE-WITH-TRAILER-LINK

## About

**THMastery** is a 2D narrative CRPG inspired by *Disco Elysium*. You play a new student at THM whose studies, conversations and decisions determine which paths through the game are available. There is no combat: challenges are solved through dialogue, skill checks, items and exploration.

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

1. Download `THMastery_Windows.zip` from the [latest release](https://github.com/Thodorr/THMastery/releases/latest).
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
- **Data-driven content:** items, checks and quests are Godot resources (`Units/`), so new content can be added without touching engine code
- **Runtime content loading:** a content factory and DLC menu integrate additional content into the running game

## Running the project

1. Install **Godot Engine 3.5**.
2. Clone this repository.
3. Import `project.godot` in the Godot Project Manager.
4. Open the project and choose **Run Project** or press **F5**.

Dialogic is included in `addons/dialogic`. If Godot reports a missing plugin after importing the project, check that it is enabled under **Project → Project Settings → Plugins**.

When exporting, keep `*.json` in the export preset's include filter, otherwise the skill table in `Data/` is missing from the build.

## Documentation

- **Game Design Document:** [docs/THMastery_GDD.pdf](docs/THMastery_GDD.pdf)
- **Project wiki:** design and development notes in the [wiki](https://github.com/Thodorr/THMastery/wiki) (work in progress)

## Team

<!-- Fill in names, roles and profile links. -->

| Name | Role |
| --- | --- |
| Tom | REPLACE: role |
| REPLACE | REPLACE |

Developed as an integration project in the Bachelor's program at [Technische Hochschule Mittelhessen (THM)](https://www.thm.de).

## Assets and licences

THMastery uses third-party assets, primarily from LimeZu's *Modern* collections. These assets have their own licence terms and are not automatically covered by a licence for this repository's source code.

Before redistributing the project, please check the terms for all included assets and keep the corresponding credits and licences with the project.

<!-- Add credits for the music tracks and any other third-party assets here. -->