# Mein Wörterbuch 🇩🇪

Il mio vocabolario di tedesco, sempre a portata di mano da PC e telefono.

**👉 Sito: https://emanuele-clc.github.io/deutsch/**

Repo: https://github.com/emanuele-clc/deutsch

## Cosa c'è

- **Parole**: articolo (der/die/das colorato), plurale o forme verbali, pronuncia, traduzione, frase d'esempio e categoria. Ricerca e filtro per categoria.
- **🔊 Audio**: pronuncia tedesca con la voce del dispositivo.
- **Ripasso**: flashcard con ripetizione spaziata, in direzione DE → IT o IT → DE.
- **Grammatica**: schede rapide su articoli e casi, sein/haben, ordine delle parole, pronuncia.
- **Sync**: le parole vengono salvate in `words.json` in questo repo, quindi PC e telefono restano allineati.

## Uso quotidiano

1. Apri il sito e premi **+ Nuova parola**.
2. Compila i campi e salva: dopo un secondo circa il sito aggiorna `words.json` su GitHub (in alto sotto il titolo compare "Sincronizzato ✓").
3. Usa **Ripasso** un po' ogni giorno: poche parole, ma spesso.

## Configurare un nuovo dispositivo (una volta sola)

1. Su GitHub: Settings → Developer settings → Personal access tokens → **Fine-grained tokens** → Generate new token.
2. Repository access: **Only select repositories** → `deutsch`.
3. Permissions → Repository permissions → **Contents: Read and write**.
4. Copia il token, apri il sito, vai su **⚙️ Sync**, incollalo e premi **Salva token**.
5. Sul telefono: "Aggiungi a schermata Home" per averlo come un'app.

Il token resta solo nel browser di quel dispositivo e non viene mai scritto nel repo. Se scade, ne generi uno nuovo e lo reincolli.

## Se qualcosa non va

- **"Token non valido?" o errore di sync**: controlla che il token sia limitato al repo `deutsch` e abbia *Contents: Read and write*.
- **Non vedo le parole nuove sull'altro dispositivo**: vai su ⚙️ Sync → **Sincronizza ora**.
- **Offline**: il sito usa la copia locale e sincronizza appena torna la connessione.
- **Backup**: ⚙️ Sync → **Esporta JSON**. Per ripristinare, **Importa JSON**.

## File

| File | A cosa serve |
|---|---|
| `index.html` | Tutto il sito (HTML, CSS e JS in un file) |
| `words.json` | Il vocabolario. Si può anche modificare a mano da GitHub |
| `README.md` | Questa guida |

## Formato di `words.json`

```json
{
  "id": "a1",
  "art": "das",
  "de": "Haus",
  "pl": "Häuser",
  "ipa": "haus",
  "it": "casa",
  "ex": "Das Haus ist groß.",
  "cat": "casa",
  "box": 0,
  "due": 0
}
```

`box` e `due` servono al ripasso (livello e prossima data): non serve toccarli.

## Note

- Il repo è pubblico, quindi le parole sono visibili a chiunque.
- Il sito funziona solo dall'indirizzo `github.io`, perché ricava utente e repo dall'URL.
