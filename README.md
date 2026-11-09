# File per il montaggio

Pacchetto di file usato dalla skill **monta-video** del Content Builder Kit di [diMarketing](https://dimarketing.it).

La skill scarica il pacchetto da sola al primo montaggio. Il cliente non deve scaricare niente. Se il download automatico non riesce, il file si scarica a mano dalla pagina [Releases](https://github.com/eggertz/dimarketing-video/releases).

## Cosa contiene

Il file `file-per-il-montaggio.zip`, nella release v1, contiene:

| Cartella | Cosa serve |
| --- | --- |
| `modello-trascrizione/` | Trascrive il video in italiano e dà il tempo di ogni parola: serve per tagliare gli errori e per i sottotitoli |
| `font/` | Montserrat Medium, il font dei sottotitoli quando il cliente non ha un suo stile |
| `licenze/` | Le licenze dei file qui sopra |

## Versioni

Ogni versione del pacchetto è una release a parte (v1, v2...). Una release pubblicata non si modifica: se cambia un file, esce una release nuova e la skill viene aggiornata per puntare a quella. Così chi usa una versione precedente della skill continua a funzionare.

## Provenienza e crediti

Il pacchetto non contiene software scritto da diMarketing: raccoglie file open source, distribuiti con le loro licenze.

| File | Autore | Licenza | Fonte |
| --- | --- | --- | --- |
| Modello di trascrizione Whisper | OpenAI | MIT | [openai/whisper](https://github.com/openai/whisper) |
| Conversione del modello per faster-whisper | SYSTRAN | MIT | [SYSTRAN/faster-whisper](https://github.com/SYSTRAN/faster-whisper) |
| Font Montserrat | The Montserrat Project Authors | SIL Open Font License 1.1 | [JulietaUla/Montserrat](https://github.com/JulietaUla/Montserrat) |

Il testo completo di ogni licenza è nella cartella `licenze/` dello zip e di questo repository.

Il montaggio usa anche [FFmpeg](https://ffmpeg.org), che non è incluso nel pacchetto: è già presente nello spazio di lavoro di Claude.

Grazie a chi ha creato e condiviso questi strumenti.
