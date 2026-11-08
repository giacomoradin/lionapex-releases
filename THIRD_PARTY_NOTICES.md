# Componenti di terzi (Third-Party Notices)

LIONApex è distribuito sotto licenza **MIT** (vedi `LICENSE`). Third-party components used by LIONApex are listed below; full license texts are in `THIRD_PARTY_LICENSES.txt`.

I testi completi, le righe di copyright di ogni pacchetto e l'elenco di tutte le dipendenze stanno in **`THIRD_PARTY_LICENSES.txt`**, generato da `strumenti/licenze_terzi.py` dai file di licenza dei pacchetti. Questa pagina riporta solo i componenti principali.

## Componenti principali

| Componente | Ruolo | Licenza | Copyright (dal file di licenza) |
|---|---|---|---|
| **libopus** 1.6.1, tramite `opusic-sys` 0.7.5 | Decodifica Opus | BSD-3-Clause | Xiph.Org, Skype Limited e altri (testo in `opus/COPYING`) |
| **`wavicle`** 0.1.0 | Decodifica WavPack | MIT OR Apache-2.0 | Copyright (c) 2026 Mark |
| **`ape-decoder`** 0.3.2 | Decodifica Monkey's Audio (APE) | MIT OR Apache-2.0 | Copyright (c) 2026 ombs.io |
| **Symphonia** 0.6.1 | Decodifica FLAC, WAV, ALAC, MP3, AAC, Vorbis | MPL-2.0 | nessuna riga di copyright nel file |
| **`tauri`** 2.11.5 | Runtime applicativo desktop | Apache-2.0 OR MIT | Copyright (c) 2017 - Present Tauri Apps Contributors |
| **`wasapi`** 0.24.0 | Uscita WASAPI su Windows | MIT | Copyright (c) 2020 Henrik Enquist |
| **`windows-sys`** (più versioni) | Binding alle API di Windows | MIT OR Apache-2.0 | Copyright (c) Microsoft Corporation. |
| **`lofty`** 0.25.1 | Lettura dei tag, ReplayGain | MIT OR Apache-2.0 | nessun file di licenza nel pacchetto: vale il campo `license` |
| **three** 0.186.0 | Grafica 3D dell'interfaccia | MIT | Copyright © 2010-2026 three.js authors |
| **pdfjs-dist** 5.7.284 | Lettura dei PDF nell'interfaccia | Apache-2.0 | nessuna riga di copyright nel file |

## Copyleft (MPL-2.0)

Symphonia e le sue sottocrate sono distribuite sotto **Mozilla Public License 2.0**. Il codice sorgente è disponibile su: https://github.com/pdeljanov/Symphonia.

Symphonia and its sub-crates are licensed under MPL-2.0; their source code is available at https://github.com/pdeljanov/Symphonia.

## ASIO

La funzionalità `asio` è spenta di default e non è abilitata nelle build di rilascio. Quando è attiva:

ASIO is a trademark of Steinberg Media Technologies GmbH, registered in Europe and other countries.
