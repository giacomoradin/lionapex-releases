# LIONApex — Master your Signal 🎵

[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-0078D6.svg)](https://github.com/giacomoradin/lionapex-releases/releases)
[![Audio Engine](https://img.shields.io/badge/Audio%20Engine-Rust%20WASAPI%20%7C%20ALSA%20%7C%20CoreAudio-dea584.svg)](https://github.com/giacomoradin/lionapex-releases)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

**LIONApex** (Lossless Input Output Node) è un riproduttore musicale ad alte prestazioni con architettura bit-perfect nativa, progettato per audiofili e amanti della musica pura.

---

## 📥 Download Ufficiali

Scarica l'eseguibile adatto al tuo sistema operativo dall'ultima release:

👉 **[Vai alla Pagina di Download (Ultima Release)](https://github.com/giacomoradin/lionapex-releases/releases/latest)**

### Guida ai file disponibili:

| Sistema Operativo | File da Scaricare | Descrizione |
| :--- | :--- | :--- |
| **Windows 10 / 11** | `LIONApex_*_x64-setup.exe` | Installer ufficiale per Windows (64-bit) |
| **Arch Linux / Manjaro / Fedora / Linux generico** | `LIONApex_*_amd64.AppImage` | Pacchetto universale autonomo (funziona su qualsiasi distro) |
| **Debian / Ubuntu / Linux Mint** | `LIONApex_*_amd64.deb` | Pacchetto DEB nativo per distribuzioni Debian-based |
| **macOS (Intel & Apple Silicon)** | `LIONApex_*_x64.dmg` | Immagine disco con applicazione macOS nativa |

> ⚠️ **IMPORTANTE: Cosa sono i file con estensione `.sig`?**  
> I file che terminano per `.sig` (es. `LIONApex_0.1.0_x64-setup.exe.sig`) **NON sono eseguibili per Mac o Linux**.  
> Sono firme crittografiche Minisign utilizzate in background dal motore di auto-aggiornamento (Tauri Updater) per verificare che l'eseguibile sia integro e autentico prima di installare gli aggiornamenti. Gli utenti **non devono scaricare né aprire i file `.sig`**.

---

## 🚀 Istruzioni di Installazione

### 🪟 Windows (10 o 11 a 64 bit)
1. Scarica il file `LIONApex_*_x64-setup.exe`.
2. Fai doppio clic per avviare l'installazione guidata.
   * *Nota Windows SmartScreen:* Se Windows mostra l'avviso *"PC protetto da Windows"* (dovuto all'assenza di un certificato EV a pagamento per sviluppatori indipendenti), fai clic su **"Ulteriori informazioni"** e poi su **"Esegui comunque"**.
3. Al termine dell'installazione, avvia **LIONApex** dal menu Start o dal desktop.

### 🐧 Linux (Arch Linux, Manjaro, Fedora, openSUSE)
1. Scarica il file `LIONApex_*_amd64.AppImage`.
2. Apri il terminale nella cartella di download e rendi eseguibile il file:
   ```bash
   chmod +x LIONApex_*_amd64.AppImage
   ```
3. Avvia l'applicazione con un doppio clic oppure da terminale:
   ```bash
   ./LIONApex_*_amd64.AppImage
   ```
   *(Opzionale: puoi installare `appimagelauncher` con `sudo pacman -S appimagelauncher` su Arch Linux per integrarlo automaticamente nel menu di sistema).*

### 🐧 Debian / Ubuntu / Linux Mint
1. Scarica il file `LIONApex_*_amd64.deb`.
2. Installa il pacchetto tramite terminale:
   ```bash
   sudo dpkg -i LIONApex_*_amd64.deb
   sudo apt-get install -f   # Risolve eventuali dipendenze di sistema
   ```
3. Avvia LIONApex dall'elenco delle applicazioni.

### 🍎 macOS
1. Scarica il file `LIONApex_*_x64.dmg`.
2. Fai doppio clic sul file scaricato e trascina l'icona di **LIONApex** nella cartella **Applicazioni**.
3. Al primo avvio, se Gatekeeper segnala che l'applicazione proviene da uno sviluppatore non identificato:
   * Fai clic con il tasto destro sull'icona di LIONApex in Applicazioni -> Seleziona **Apri** -> Conferma facendo clic su **Apri**.

---

## 🧙‍♂️ Primo Avvio: Setup Wizard Guidato

Alla prima apertura su un nuovo computer, LIONApex apre automaticamente la **Procedura Guidata di Benvenuto**:

1. **Cartelle Musicali**:
   - **Cartella Locale / USB**: se hai la tua musica su una chiavetta USB (es. unità `E:\` o cartella locale), LIONApex la utilizzerà a latenza zero.
   - **Cartella Cloud / Google Drive**: cartella cloud di riserva (es. `G:\My Drive\MUSIC_flac_wav_mp3`).
   - **Cartella Download Brani**: la cartella dove salvare i nuovi brani scaricati.
2. **Database Archivio (`music.db`)**:
   - Clicca **"🔍 Trova in automatico"** per far scansionare all'istante tutte le unità connesse (`C:`..`Z:`) e collegare il database della tua chiavetta USB.
   - Oppure clicca **"📥 Importa nel PC"** per copiare il database in locale sul computer e renderlo sempre accessibile anche a chiavetta scollegata.
   - Oppure clicca **"✨ Crea archivio vuoto"** se parti da zero.
3. **Servizi Esterni & Chiavi API (Completamente OPZIONALI)**:
   - **Google Gemini AI**: attiva se desideri generare playlist tematiche intelligenti analizzando la tua libreria con i modelli Gemini.
   - **ListenBrainz**: attiva per inviare la cronologia degli ascolti.
   - *Tutte le chiavi sono personali e vengono memorizzate unicamente sul tuo computer locale (`%LOCALAPPDATA%\LIONApex\credenziali.json`).*
4. Clicca **"Salva e Avvia"**: la libreria caricherà immediatamente tutti i tuoi brani, copertine e testi!

> 💡 Puoi riaprire il Setup Wizard o modificare queste impostazioni in qualsiasi momento dal pulsante **"Configurazione Guidata"** nella scheda **Impostazioni**.

---

## ⚡ Caratteristiche Tecniche di LIONApex

* 🎯 **Uscita Bit-Perfect Reale:**
  - **Windows:** WASAPI Esclusiva (bypass totale del mixer di sistema e dei ricampionamenti Windows).
  - **Linux:** ALSA Direct Hardware a campioni esatti e compatibilità PipeWire a bassa latenza.
  - **macOS:** CoreAudio HAL bit-perfect nativo.
* 🦀 **Motore Audio Nativo Rust (`audio-core`):** Decodifica autonoma ad altissima efficienza con Symphonia (FLAC, WAV, ALAC, MP3, AAC, OGG, Vorbis) con thread realtime MMCSS Pro Audio.
* 🎧 **Calibrazione Cuffie AutoEq:** Database integrato con migliaia di curve di compensazione Harman / diffuse-field per cuffie e auricolari.
* 🎚️ **Master Lab & DSP:** Equalizzatore parametrico a fase lineare a 10 bande, dither TPDF e limitatore True-Peak.
* 📊 **Deck 3D Immersion & Spettro RTA:** Analizzatore di spettro FFT a 64 bande con rendering fluido e cadenza adattiva intelligente.
* 📜 **Testi Sincronizzati:** Ricerca e sincronizzazione automatica dei testi (.lrc) in tempo reale.

---

*LIONApex — Master your signal. Designed and engineered by Giacomo Radin.*