# Usagi Yojimbo — correzione del sentiero / uphill-path correction

23 November 2026 · Update for the existing R8 package.

[Download ZIP — 38.2 MB](plus64-usagi-correzione-sentiero.zip)

## Italiano

Chiudi il gioco ed estrai lo ZIP nella cartella della R8 che contiene `xplus4.exe`, confermando la sostituzione dei file. Avvia `AVVIA_USAGI_FLUIDO.cmd`, seleziona **F1 → GAME**, poi **F7** e comincia una nuova partita.

L'aggiornamento corregge il disallineamento dei colori quando il sentiero sale alla fine del primo scenario. La posizione dei materiali segue ora la matrice effettivamente visualizzata e il fine scroll TED. Mantiene i colori e gli asset approvati, l'avvio con audio SDL e filtro CRT disattivato, e il limite **64+16 KiB = 81.920 byte**. Include eseguibile e disco aggiornati, sorgenti completi corrispondenti e un'appendice tecnica SDK in italiano e inglese.

Per applicare il nuovo codice usa una nuova partita: i vecchi snapshot contengono anche il vecchio programma. Il manuale tecnico completo della R8 resta valido per i nodi precedenti; l'appendice documenta il nuovo flag opzionale Scenery23.

Verifiche: SDK e snapshot sui due profili; 60 fotogrammi del tratto finale, fermi e in movimento, con zero errori nei pixel dei materiali, del sentiero e del terreno; quattro fixture dei costruttori speciali; avvio e confronti dell'eseguibile Windows tramite Wine.

## English

Close the game and extract the ZIP into the R8 folder containing `xplus4.exe`, replacing the supplied files. Run `AVVIA_USAGI_FLUIDO.cmd`, select **F1 → GAME**, then **F7**, and start a new game.

The update fixes colour/material drift near the uphill path at the end of the first scene. Material coordinates now follow the matrix actually displayed and the native TED fine scroll. It retains the approved artwork, the SDL-audio/pixel launch profile and the **64+16 KiB = 81,920-byte** guest-memory limit. Updated executable and disk, complete corresponding sources, and Italian/English technical SDK addenda are included.

Start a new game to use the update: older snapshots also contain the older game program. The complete R8 technical manual remains valid for legacy nodes; the addendum documents the optional Scenery23 flag.

Validation covers SDK/snapshot tests on both machine profiles, 60 moving/idle frames of the final path with zero material/path/static-terrain pixel errors, four special-constructor fixtures, and Windows executable startup/replay comparisons through Wine. This is finite Linux/Wine coverage.

SHA-256: `136482c773f45469283365798ca363839ec7091043b33c8f2e769fd177a507e2`.
