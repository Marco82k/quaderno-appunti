# Quaderno Appunti

Trascrivi o riassumi con Gemini i PDF dei tuoi appunti e delle slide e la registrazione audio delle lezioni, e organizza tutto in un quaderno per materia con flashcard, quiz e tutor. Gira sul tuo PC e si usa dal browser.

**[⬇️ Scarica l'ultima versione per Windows](https://github.com/Marco82k/quaderno-appunti/releases/latest)**: in *Assets* trovi **QuadernoAppunti-Setup.exe**.

## Come installare (Windows 10/11)

1. Scarica **QuadernoAppunti-Setup.exe** qui sotto (in *Assets*) e aprilo.
2. Windows potrebbe dire *"Windows ha protetto il PC"*: l'app non è firmata da un'azienda. Premi **Ulteriori informazioni → Esegui comunque**.
3. Segui l'installazione: non servono i permessi di amministratore. Alla fine l'app si apre nel browser.
4. La prima volta ti chiede una **chiave API di Google Gemini**, gratuita: creala su [Google AI Studio](https://aistudio.google.com/apikey) con il tuo account Google (*Create API key*) e incollala.

Per riaprirla usa l'icona **Quaderno Appunti** sul desktop o nel menu Start. Si apre una finestra nera: lasciala aperta mentre usi l'app, chiuderla spegne l'app.

## Dove sono i dati

Il quaderno, la chiave e le impostazioni sono in `%APPDATA%\QuadernoAppunti` (nel menu Start: *Cartella dei dati e impostazioni*). Aggiornare o disinstallare l'app non li cancella.

## Modalità utente e admin

L'app parte in **modalità utente**. La **modalità admin** aggiunge la scelta del modello Gemini, i limiti, le chiavi e il Pannello admin. Per cambiarla:

- apri `impostazioni.ini` nella cartella dei dati e scrivi `modalita = admin` (oppure `utente`), poi riapri l'app;
- oppure dal terminale, nella cartella dell'app (`%LOCALAPPDATA%\Programs\QuadernoAppunti`):
  ```
  QuadernoAppunti.exe --admin
  QuadernoAppunti.exe --utente
  QuadernoAppunti.exe --modalita
  ```
  `--modalita` mostra la modalità attuale senza avviare l'app.
