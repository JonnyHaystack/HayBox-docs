# Overview

HayBox is a modular, cross-platform firmware for digital or mixed analog/digital controllers, primarily targeted at [B0XX](https://b0xx.com)-style controllers.

[![GitHub issues](https://img.shields.io/github/issues/JonnyHaystack/HayBox)](https://github.com/JonnyHaystack/HayBox/issues)
[![GitHub pull requests](https://img.shields.io/github/issues-pr/JonnyHaystack/HayBox)](https://github.com/JonnyHaystack/HayBox/pulls)

## Features

Features include:

- Cross platform support:
    - RP2040 (e.g. Raspberry Pi Pico)
    - 16MHz AVR MCUs (e.g. ATMega32U4 which several Arduinos are based on)
- Supports many existing controllers/PCBs, e.g. B0XX, LBX, Smash Box, Crane's
  GCCPCB/Model S
- Supports a variety of communication backends which can be used either separately or in conjunction with each other:
    - XInput
    - DInput
    - GameCube console
    - Nintendo 64 console
    - Nintendo Switch console
    - B0XX input viewer
- Supports a variety of "input sources" which can be used in conjunction to create mixed input controllers:
    - Buttons/switches wired directly to GPIO pins
    - Switch matrix (as typically found in keyboards)
    - Wii Nunchuk
    - GameCube controller
- Melee mode up to date with B0XX V3 specifications
- Existing modes for popular games (e.g. Melee, Project M, Ultimate, Rivals of Aether, traditional fighting games)
- Easy to create new controller modes (or keyboard modes) for different games
- USB keyboard game modes for games that lack gamepad support
- Fully customisable SOCD cleaning, allowing you to configure SOCD button pairs (e.g. left/right, up/down) for each controller/keyboard mode, and also easily change the SOCD resolution method for each SOCD pair
- Switch modes on the fly without unplugging your controller
- Automatically detects whether plugged into console or USB
- Game modes and communication backends are independent entities, meaning you can use any game mode with any supported console without extra work
- Easily switch between different GameCube/N64 polling rates in order to have optimal latency on console, overclocked adapter, etc. (not necessary for Pico/RP2040)