# Informativa sulla privacy — LIONApex e LIONApex Island

*Ultimo aggiornamento: 8 novembre 2026. English version below.*

LIONApex (il player) e LIONApex Island (l'isola) sono programmi gratuiti che girano sul tuo computer. Chi li
sviluppa **non gestisce server**, non riceve dati da chi li usa e non ha accesso a quello che fai con i programmi.
Non c'e' telemetria, non ci sono statistiche d'uso, identificatori pubblicitari o cookie di profilazione.

## Che cosa resta sul tuo computer
Libreria, cronologia d'ascolto, playlist, impostazioni, indice della ricerca, cronologia degli appunti e misure dei
brani restano nelle cartelle dei programmi sul tuo disco. Le chiavi che inserisci (per esempio quella di Google
Gemini) e i segreti del telecomando sono cifrati con la protezione dati di Windows (DPAPI), legata al tuo utente.
Per cancellare tutto basta disinstallare i programmi ed eliminare le loro cartelle in `%LOCALAPPDATA%`.

## Quando i programmi si collegano a Internet
Alcune funzioni contattano servizi di terzi **direttamente dal tuo computer**. Quel servizio vede il tuo indirizzo
IP e cio' che la funzione gli chiede; i suoi trattamenti sono regolati dalla sua informativa, non da questa.

| Funzione | Servizio | Che cosa riceve |
|---|---|---|
| Aggiornamenti automatici | GitHub | la richiesta del file della versione e il download |
| Meteo nell'isola (se attivo) | Open-Meteo | le coordinate della posizione (o la citta' cercata) |
| Testi delle canzoni | LRCLIB | artista, titolo, album e durata del brano |
| Informazioni e foto degli artisti | MusicBrainz, Wikidata, Wikipedia/Wikimedia | il nome dell'artista o del disco |
| Scrobbling (se lo attivi) | ListenBrainz, Last.fm | i brani ascoltati, con la tua chiave |
| Assistente con Gemini (se inserisci una chiave) | Google | la richiesta e i dati dei brani necessari |
| Mini player e iscrizioni YouTube | YouTube (anche youtube-nocookie.com, img.youtube.com) | il video o il canale richiesto |
| Scorciatoie della ricerca | il sito che scegli di aprire | cio' che apre il tuo browser |

L'assistente locale (Ollama), il telecomando dal telefono, il renderer UPnP e il collegamento con l'estensione del
browser restano sul tuo computer o sulla tua rete locale. Le funzioni che usano un servizio esterno si possono non
usare o spegnere.

## I tuoi diritti
Poiche' chi sviluppa i programmi non raccoglie dati personali, non c'e' nulla da consultare, correggere o
cancellare presso di lui: i dati sono sul tuo dispositivo e li gestisci tu. Per i servizi di terzi elencati sopra
valgono i diritti previsti dal Regolamento (UE) 2016/679 nei confronti di ciascun servizio.

Contatti: tramite la pagina del progetto su GitHub (sezione Issues).

---

# Privacy notice — LIONApex and LIONApex Island

*Last updated: 8 November 2026.*

LIONApex (the player) and LIONApex Island are free programs that run on your computer. The developer **runs no
servers**, receives no data from users and has no access to what you do with the programs. There is no telemetry,
no usage statistics, no advertising identifiers and no profiling cookies.

**What stays on your computer:** library, listening history, playlists, settings, search index, clipboard history
and track measurements stay in the programs' folders on your disk. Keys you enter (e.g. a Google Gemini key) and the
remote-control secrets are encrypted with Windows data protection (DPAPI), bound to your user account.

**When the programs connect to the Internet:** some features contact third-party services **directly from your
computer**; that service sees your IP address and what the feature requests, under its own privacy policy:
GitHub (updates), Open-Meteo (weather: location coordinates or the city you search), LRCLIB (lyrics: artist, title,
album, duration), MusicBrainz / Wikidata / Wikipedia / Wikimedia (artist and album information), ListenBrainz and
Last.fm (scrobbling, if enabled), Google Gemini (assistant, if you enter a key), YouTube (mini player and channel
feeds), and any website you choose to open from the search shortcuts. The local assistant (Ollama), the phone remote,
the UPnP renderer and the browser-extension link stay on your computer or local network.

**Your rights:** since the developer collects no personal data, there is nothing to access, correct or erase on
the developer's side; your data is on your device. Your GDPR rights apply towards each third-party service above.
