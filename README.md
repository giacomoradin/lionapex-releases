# LIONApex — Master your Signal 🎵

[![Platform](https://img.shields.io/badge/Platform-Windows%20x64-0078D6.svg)](https://github.com/giacomoradin/lionapex-releases/releases)
[![Engine](https://img.shields.io/badge/Audio%20Engine-Rust%20WASAPI%20Exclusive-dea584.svg)](https://github.com/giacomoradin/lionapex-releases)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

**LIONApex** (Lossless Input Output Node) is a modern, high-performance, bit-perfect music player built for audiophiles and music lovers.

---

## ⚡ Caratteristiche Principali

* 🎯 **Uscita Bit-Perfect WASAPI Esclusiva:** Nessun ricampionamento o alterazione dal mixer di sistema di Windows. Consegna campioni esatti al DAC.
* 🦀 **Motore Audio Nativo in Rust (audio-core):** Decodifica in puro Rust con Symphonia per FLAC, WAV, ALAC, MP3, AAC, OGG e Vorbis. Zero crash, memoria controllata e thread audio ad alta priorità realtime (MMCSS Pro Audio).
* 🎧 **Calibrazione Cuffie AutoEq:** Database integrato con migliaia di profili di equalizzazione parametrici misurati per cuffie over-ear, in-ear ed earbuds.
* 🎚️ **Equalizzatore Parametrico & Limitatore True-Peak:** 10 bande con filtri biquad ad alta precisione e dither TPDF.
* 📊 **Analizzatore di Spettro RTA & Deck 3D Immersion:** Spettro a 64 bande calcolato con FFT reale e visualizzazione 3D ad alta frequenza di fotogrammi con risparmio energetico intelligente.
* 💾 **Smart Mount & Priorità Locale:** Riconosce automaticamente copie della musica su chiavette USB o dischi locali veloci per la riproduzione immediata a latenza zero, con sincronizzazione e fallback su Google Drive.
* 📜 **Testi Sincronizzati:** Ricerca e visualizzazione automatica dei testi sincronizzati (.lrc) tramite LRCLIB con cache persistente.
* 🔄 **Aggiornamenti Continui Silenziosi:** Sistema di aggiornamento automatico firmato digitalmente, senza dover disinstallare o reinstallare l'app.

---

## 📥 Download e Installazione

Scarica l'ultimo installer per Windows:

👉 **[Scarica LIONApex Setup (.exe)](https://github.com/giacomoradin/lionapex-releases/releases/latest)**

1. Scarica ed esegui LIONApex_Setup.exe.
2. Segui la procedura guidata (richiede Windows 10 o Windows 11 a 64 bit).
3. Apri LIONApex e goditi la tua musica bit-perfect!

---

## 🛠️ Requisiti di Sistema

* **Sistema Operativo:** Windows 10 (aggiornato) o Windows 11 (64-bit)
* **WebView2 Runtime:** Già preinstallato su Windows 10 e 11
* *(Versioni per Linux/Debian e macOS in arrivo tramite pipeline CI/CD)*

---

*LIONApex — Designed and engineered by Giacomo Radin.*