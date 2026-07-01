# Control Systems Notes — setup

Blog minimale (Jekyll) per appunti brevi di controlli automatici / GNC.
Zero build manuale: GitHub Pages genera il sito da solo a ogni push.

## Come pubblicarlo (una volta sola)

1. Vai su github.com e crea un nuovo repository pubblico chiamato
   **`control-systems-notes`** (o il nome che preferisci — se cambi nome,
   aggiorna anche `baseurl` in `_config.yml`).

2. Carica tutti i file di questa cartella nel repo (drag & drop dei file
   dalla pagina del repo su GitHub va benissimo, oppure via git da terminale
   se preferisci).

3. Nel repo, vai su **Settings → Pages**, e sotto "Build and deployment"
   seleziona come source: **Deploy from a branch**, branch `main`, folder
   `/ (root)`. Salva.

4. Dopo 1-2 minuti il sito sarà live su:
   `https://TUO_USERNAME.github.io/control-systems-notes/`

5. Apri `_config.yml` e sostituisci `danieledigiamberardino` nel campo `url`
   con il tuo username GitHub esatto se diverso, e verifica che `baseurl`
   corrisponda al nome del repo che hai scelto.

## Come scrivere un nuovo post

1. Duplica il file dentro `_posts/` che fa da esempio
   (`2026-07-01-il-margine-di-fase-in-due-minuti.md`).

2. Rinomina il nuovo file seguendo lo schema:
   `AAAA-MM-GG-titolo-breve-con-trattini.md`
   (la data nel nome del file è obbligatoria per Jekyll, determina
   l'ordinamento cronologico dei post).

3. Nell'intestazione (tra i tre trattini `---`) aggiorna `title` e `tags`.

4. Scrivi il contenuto in Markdown normale. Per le formule:
   - inline: `$\zeta$` per una variabile nel testo
   - a blocco: `$$ formula $$` su una riga a parte

5. Fai commit e push. Entro 1-2 minuti il post è online.

## Struttura consigliata per ogni post (facoltativa ma utile)

- **Cos'è** — definizione in 2-3 righe
- **Formula** — la relazione chiave
- **Perché conta** — intuizione pratica / quando torna utile
- **Nota a margine** (opzionale) — un'imprecisione comune o un caso limite

Tenerti a questo schema rende la scrittura quasi meccanica: 15-20 minuti a
post, non un impegno da articolo accademico.
