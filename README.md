# fpiantini.it  - In Pausa

Questo repository contiene il codice sorgente del sito personale di Francesco Piantini.

Il sito è realizzato con [Hugo]. Per una guida su come installare e usare Hugo vedere la pagina [getting started] sul sito di Hugo. Nel seguito un riassunto veloce dei comandi principali.

## Come aggiungere contenuto

Prerequisito: un'installazione funzionante di [Hugo]. Deve essere disponibile il comando `hugo`:

Per creare un nuovo articolo usare il comando:

```bash
hugo new posts/nuovo-post.md
```

Viene creato un file `content/posts/nuovo-post.md`. Il file può essere editato per aggiungere il contenuto desiderato.

Una volta che l'articolo è pronto per la pubblicazione, modificare il campo `draft` da `true` a `false` nell'header dello stesso.

## Come visualizzare il sito durante lo sviluppo

Lanciare il server Hugo con il comando:

```bash
hugo server -D
```

L'opzione `-D` è usata per permettere la visualizzazione anche degli articoli in stato draft.

## Come pubblicare l'aggiornamento del sito

Per generare la versione statica del sito con il contenuto aggiornato dare il comando:


```bash
hugo
```

Usare l'opzione `-D` se si vogliono pubblicare anche le pagine ancora in stato draft. Il risultato è generato all'interno della directory `public`, il cui contenuto può essere copiato nella directory utilizzata per pubblicare il sito sulla macchina utilizzata per il web hosting


[Hugo]: https://gohugo.io/
[getting started]: https://gohugo.io/getting-started/quick-start/