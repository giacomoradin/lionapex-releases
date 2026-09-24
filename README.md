<div align="center">

# 🎵 LIONApex — Master your Signal

### Il Player Audio Lossless Bit-Perfect ad Alta Precisione

[![Latest Release](https://img.shields.io/github/v/release/giacomoradin/lionapex-releases?color=FF6600&label=Release%20Stabile&logo=github)](https://github.com/giacomoradin/lionapex-releases/releases/latest)
[![Platform](https://img.shields.io/badge/Piattaforme-Windows%20%7C%20Linux%20%7C%20macOS-0078D6.svg?logo=windows&logoColor=white)](https://github.com/giacomoradin/lionapex-releases/releases)
[![Audio Engine](https://img.shields.io/badge/Audio%20Engine-WASAPI%20%7C%20ALSA%20%7C%20CoreAudio-dea584.svg?logo=rust&logoColor=white)](https://github.com/giacomoradin/lionapex-releases)
[![Auto Updater](https://img.shields.io/badge/Auto--Updater-Minisign%20Ed25519-success.svg?logo=shield&logoColor=white)](https://github.com/giacomoradin/lionapex-releases)
[![Licenza](https://img.shields.io/badge/Licenza-MIT-blue.svg)](LICENSE)

<p align="center">
  <b>LIONApex</b> (Lossless Input Output Node) è progettato per audiofili e amanti del suono non compresso. Offre un'esperienza d'ascolto senza compromessi, con bypass del mixer di sistema operativo, routing bit-perfect a bassissima latenza, equalizzazione parametrica da studio e interfaccia adattiva.
</p>

[📥 Scarica Ora](#-download-ufficiali--canali-di-rilascio) • [🧙‍♂️ Setup Wizard](#-primo-avvio-setup-wizard-guidato) • [💼 Versioni Portable](#-come-usare-le-versioni-portable) • [💬 Community & Feedback](#-community-segnalazioni-e-feedback)

</div>

---

## 📥 Download Ufficiali & Canali di Rilascio

Scegli il canale di rilascio e la versione adatta alle tue esigenze:

### 🟢 Canale Stabile (Consigliato)
Contiene le versioni testate e pronte per l'uso quotidiano.

| Sistema Operativo | Tipo di Pacchetto | File da Scaricare | Note d'Installazione |
| :--- | :--- | :--- | :--- |
| **🪟 Windows (10/11 64-bit)** | **Installer Guidato** | [`LIONApex_*_x64-setup.exe`](https://github.com/giacomoradin/lionapex-releases/releases/latest) | Installazione con integrazione nel menu Start e scorciatoie |
| **🪟 Windows (10/11 64-bit)** | **💼 Versione Portable** | [`LIONApex_x64_Portable.zip`](https://github.com/giacomoradin/lionapex-releases/releases/latest) | **Zero installazione**: estrai e avvia, ideale per chiavette USB |
| **🐧 Linux (Universale)** | **💼 Portable AppImage** | [`LIONApex_*_amd64.AppImage`](https://github.com/giacomoradin/lionapex-releases/releases/latest) | Funziona su **qualsiasi distro** (Arch, Manjaro, Fedora, openSUSE, Debian, Ubuntu) |
| **🐧 Linux (Debian/Ubuntu)** | **Pacchetto di Sistema** | [`LIONApex_*_amd64.deb`](https://github.com/giacomoradin/lionapex-releases/releases/latest) | Installazione nativa gestita da APT/dpkg |
| **🍎 macOS (Apple Silicon & Intel)** | **Immagine Disco** | [`LIONApex_*_aarch64.dmg` / `x64.dmg`](https://github.com/giacomoradin/lionapex-releases/releases/latest) | Trascina in *Applicazioni* |

👉 **[Apri la Pagina di Download dell'Ultima Release](https://github.com/giacomoradin/lionapex-releases/releases/latest)**

---

### 🟡 Canale Beta & Anteprime (Funzionalità Sperimentali)
Se desideri provare in anteprima i nuovi moduli audio DSP, miglioramenti grafici o codec sperimentali:
- Consulta i rilasci contrassegnati con l'etichetta **Pre-release** o **Beta**:  
  👉 **[Esplora le Release Beta / Pre-release](https://github.com/giacomoradin/lionapex-releases/releases?q=prerelease%3Atrue)**

---

### 📦 Archivio Storico (Versioni Precedenti)
Hai bisogno di ripristinare una versione specifica o consultare il changelog delle versioni passate?  
👉 **[Consulta tutte le Release Precedenti](https://github.com/giacomoradin/lionapex-releases/releases)**

---

<details>
<summary><b>🔒 File Tecnici & Firme Crittografiche (Clicca per espandere — Non scaricare manualmente)</b></summary>

<br />

All'interno dell'elenco delle release potresti notare file come:
- `*.sig` (es. `LIONApex_*_setup.exe.sig`, `*.AppImage.sig`)
- `latest.json`

> ⚠️ **Importante per gli utenti:**  
> **Non scaricare questi file**. Non sono file eseguibili per Mac o Linux.  
> Sono **firme crittografiche Minisign (Ed25519)** e manifest informativi utilizzati in modo invisibile e automatico dal plugin **Tauri Auto-Updater** integrato in LIONApex. Quando apri LIONApex e verifichi gli aggiornamenti, l'applicazione legge questi file per certificare che l'aggiornamento sia autentico e non manomesso prima di installarlo.
</details>

---

## 💼 Come Usare le Versioni Portable

Le versioni **Portable** sono pensate per chi desidera usare LIONApex su computer diversi senza installare nulla nel sistema operativo:

### 🪟 Windows Portable
1. Scarica l'archivio `LIONApex_x64_Portable.zip`.
2. Estrai la cartella dove preferisci (ad esempio sul Desktop o **direttamente dentro la tua chiavetta USB** `E:\LIONApex\`).
3. Avvia `lionapex.exe` (o `LIONApex.exe`).
4. **Vantaggi**:
   - Non scrive chiavi nel registro di sistema di Windows.
   - Non richiede diritti di amministratore.
   - Se posizionato su una chiavetta USB insieme ai tuoi brani e al file `music.db`, ti permette di portare l'intero archivio musicale sempre con te su qualsiasi PC!

### 🐧 Linux Portable (AppImage)
1. Scarica `LIONApex_*_amd64.AppImage`.
2. Assegna i permessi di esecuzione:
   ```bash
   chmod +x LIONApex_*_amd64.AppImage
   ```
3. Avvia l'applicazione con un doppio clic o da terminale:
   ```bash
   ./LIONApex_*_amd64.AppImage
   ```
4. Non richiede installazione né dipendenze esterne.

---

## 🚀 Istruzioni di Installazione (Versioni con Installer)

### 🪟 Windows (10/11 a 64 bit)
1. Scarica `LIONApex_*_x64-setup.exe` ed avvialo.
2. *Nota Windows SmartScreen:* Se Windows mostra l'avviso *"PC protetto da Windows"*, clicca su **"Ulteriori informazioni"** e poi su **"Esegui comunque"**.
3. Segui la procedura guidata e avvia LIONApex.

### 🐧 Debian / Ubuntu / Linux Mint
```bash
sudo dpkg -i LIONApex_*_amd64.deb
sudo apt-get install -f   # Installa eventuali librerie mancanti se necessario
```

### 🍎 macOS
1. Scarica `LIONApex_*_aarch64.dmg` (Apple Silicon) o `x64.dmg` (Intel).
2. Fai doppio clic sul `.dmg` e trascina **LIONApex** in **Applicazioni**.
3. Al primo avvio, se compare l'avviso di Gatekeeper: fai clic destro sull'icona in Applicazioni -> **Apri** -> conferma cliccando su **Apri**.

---

## 🧙‍♂️ Primo Avvio: Setup Wizard Guidato

Alla prima apertura su un nuovo computer, LIONApex avvia la procedura guidata interattiva:

1. **Selezione Sorgenti Musicali**:
   - **Cartella Locale / USB**: seleziona la tua chiavetta USB (es. `E:\` o `E:\MUSIC_flac_wav_mp3`) o il disco locale.
   - **Cartella Google Drive**: cartella sincronizzata sul cloud di riserva.
   - **Cartella Download**: directory per i nuovi file audio scaricati.
2. **Collegamento Database Archivio (`music.db`)**:
   - Clicca **"🔍 Trova in automatico"** per scansionare istantaneamente tutte le unità USB e connettere il database esistente.
   - Clicca **"📥 Importa nel PC"** se vuoi copiare il database sul computer locale per ascoltare la musica anche quando la chiavetta non è inserita.
3. **Servizi API Opzionali (Configurabili dall'utente)**:
   - **Google Gemini AI**: per abilitare le playlist generate con intelligenza artificiale.
   - **ListenBrainz**: per inviare gli scrobble dei tuoi ascolti.
   - *Tutte le chiavi API sono private e rimangono salvate esclusivamente sul tuo computer locale.*

---

## 💬 Community, Segnalazioni e Feedback

Siamo felici di ricevere il tuo parere per rendere LIONApex sempre più fedele e piacevole da usare:

- 🐛 **Hai riscontrato un bug o un errore audio?**  
  [Apri una Segnalazione di Bug](https://github.com/giacomoradin/lionapex-releases/issues/new?template=bug_report.yml) specificando il tuo sistema operativo e DAC audio.
- 💡 **Hai un'idea per una nuova funzionalità?**  
  [Invia una Proposta di Funzionalità](https://github.com/giacomoradin/lionapex-releases/issues/new?template=feature_request.yml).
- 💬 **Vuoi condividere la tua opinione?**  
  [Invia un Feedback Generale](https://github.com/giacomoradin/lionapex-releases/issues/new?template=feedback.yml).
- 🔒 **Segnalazioni di Sicurezza:**  
  Consulta la nostra [Politica di Sicurezza (SECURITY.md)](SECURITY.md).
- 🤝 **Codice di Condotta:**  
  Ci impegniamo a garantire una community aperta, rispettosa e accogliente: [Code of Conduct](CODE_OF_CONDUCT.md).

---

## 📜 Licenza

Distribuito con licenza **MIT**. Consulta il file [`LICENSE`](LICENSE) per i dettagli completi.