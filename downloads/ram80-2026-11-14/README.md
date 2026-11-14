# plus/64 RAM80 software preview

Updated 14 November 2026. This is Meck's software prototype for a common Commodore 16 and Plus/4 platform: **64 KiB cartridge RAM + 16 KiB internal RAM = 81,920 bytes**. Sprite/cache, audio and modem payloads share that budget.

## Downloads

| File | Contents |
| --- | --- |
| [Complete Windows kit](https://raw.githubusercontent.com/abattiloro78-codex/plus64-downloads/main/downloads/ram80-2026-11-14/plus64-ram80-rev8r-completo.zip) | Modified VICE executable, required DLLs, enhanced Impossible Mission REV8R, PRISM INVADERS and two SDK demonstrations. |
| [Technical developer manual and SDK, Italian and English](https://raw.githubusercontent.com/abattiloro78-codex/plus64-downloads/main/downloads/ram80-2026-11-14/plus64-manuale-sviluppatore-ram80-it-en.zip) | Full 44-page manual and 6-page quick reference in each language, editable sources, API JSON, current source excerpts and reproducible assembly examples. |
| [English manual PDF](https://raw.githubusercontent.com/abattiloro78-codex/plus64-downloads/main/downloads/ram80-2026-11-14/PLUS64_RAM80_Developer_Manual_EN.pdf) | Complete English copy, not an abridged guide. |
| [Italian manual PDF](https://raw.githubusercontent.com/abattiloro78-codex/plus64-downloads/main/downloads/ram80-2026-11-14/Manuale_Sviluppatore_PLUS64_RAM80_IT.pdf) | Complete updated Italian manual. |
| [Optional Impossible Mission test saves](https://raw.githubusercontent.com/abattiloro78-codex/plus64-downloads/main/downloads/ram80-2026-11-14/plus64-im-rev8r-prove.zip) | All 36 pieces collected, or password completed directly at the final door. |
| [Full modified VICE GPL sources](https://raw.githubusercontent.com/abattiloro78-codex/plus64-downloads/main/downloads/ram80-2026-11-14/plus64-scenari-rev8r-sorgenti.tar.xz) | Corresponding emulator sources and build recipes. Optional for running the games. |
| [SHA256 checksums](SHA256SUMS.txt) | Digests of all downloadable files. |

## Running the software

Extract the complete kit into a **new writable folder** and run `AVVIA_PLUS64.cmd`. The menu opens the enhanced Impossible Mission version, PRISM INVADERS, the RAW8/SID SDK sample or the new material-lighting sample. Use this supplied modified VICE executable, not stock VICE. The normal game contains no preset progress.

Extract optional test saves into that same folder if wanted. `PROVA_TUTTI_PEZZI.cmd` starts with 36 collected pieces and unassembled puzzles. `PROVA_PASSWORD_TROVATA.cmd` starts with the password complete at the final door; press joystick UP.

The new executable is the qualified REV8R build with debug information removed; mapped code/data sections are identical. The accompanying checks cover Linux C16/Plus4 execution and the Windows executable under Wine. Native Windows, physical cartridge circuitry and a naturally completed full Impossible Mission mission are not claimed. An intermittent robot-shock report during searching remains unchanged by agreement; it was not reproduced in scoped checks.

## Programming

The technical manual updates the original seven chapters rather than replacing them with a game guide. It documents RAM80 aliases and ownership, protocols 05/03, CPU-driven upload ports, sprite and TED formats, SID and modem, 121 colours, nine light positions, diagonal per-ink lighting, sparse masks, scenery/compositing descriptors and complete snapshots. The updated SDK includes an independent mask example with 121 selectable highlights and north/east/front illumination.

The new visual modes are implemented in the emulator. Their physical data-access path, genlock timing, bandwidth, contention and circuit cost remain hardware-design work. This preview does not turn arbitrary C64 programs into compatible software.

The older release remains available: [software preview published 10 November](https://github.com/abattiloro78-codex/plus64-downloads/releases/tag/software-preview-2026-11-08).
