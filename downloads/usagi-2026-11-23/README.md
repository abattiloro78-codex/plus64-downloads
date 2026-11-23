# Usagi Yojimbo per plus/64 — R8, 23 November 2026

[Download the complete R8 ZIP](./plus64-usagi-yojimbo-2026-11-23-r8.zip) — 50,749,102 bytes (48.4 MiB).

Extract to a new folder, open `plus64-usagi` and launch `AVVIA_USAGI.cmd` (C16) or `AVVIA_USAGI_PLUS4.cmd` (Plus/4). Select **GAME** with F1, then start with F7. F5 selects English or Italian. Both profiles use the same D64. The Linux `.sh` launchers require separately installed Wine64 and use the supplied Windows runtime.

R8 retains the reviewed artwork and fixes actor colour ownership (including Ninja blood), foreground poles and handrails on every bridge, fast disk startup, and the Linux keyboard-map path. Bridge decks remain behind the actors. The generic renderer reuses validated temporary program work within each frame; guest RAM remains **64 KiB + 16 KiB = 81,920 bytes**, shared by all platform features. Only the active scene's colour program is loaded from disk.

Three recorded ordinary level1 views on C16 and Plus/4 used a median **29.88% less emulator CPU** in paired tests, with identical guest state and images. This measures headless CPU work with chip emulation enabled; it is not a displayed-FPS or audio-fidelity measurement. The Windows executable was tested through Wine; native Windows, physical hardware and a completed campaign are not claimed.

The tree data match the preserved published previews. [Published artwork versus captured game pixels](./usagi-alberi-concordati-confronto.png). The original separate PRACTICE arena retains its original background; the 17 reviewed scenery programs apply to GAME maps.

The ZIP includes the runtime, game, corresponding sources, editable artwork, detailed test receipts and both full technical developer manuals. Each manual has 53 pages; HTML, Markdown and quick references are included too.

- [Italian technical developer manual](./Manuale_Sviluppatore_PLUS64_RAM80_IT.pdf)
- [English technical developer manual](./PLUS64_RAM80_Developer_Manual_EN.pdf)
- [Checksums](./SHA256SUMS.txt)

The small launcher-only correction remains available for the preceding package. R8 includes it and the further corrections above.
