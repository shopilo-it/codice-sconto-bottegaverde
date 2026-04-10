# Codice sconto Bottega Verde, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Bottega Verde** da [shopilo.it](https://shopilo.it/negozi/bottegaverde.it). Restituisce **coupon Bottega Verde** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-bottegaverde](https://shopilo-it.github.io/codice-sconto-bottegaverde/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-bottegaverde
cd codice-sconto-bottegaverde
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Bottega Verde",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su cosmetici naturali",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/bottegaverde.it"
  }
]
```

## Coupon Bottega Verde disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 20% | 20% di sconto su cosmetici naturali | [shopilo.it](https://shopilo.it/negozi/bottegaverde.it) |

Codici attivi: **[shopilo.it/negozi/bottegaverde.it](https://shopilo.it/negozi/bottegaverde.it)**

## Domande frequenti

### Come utilizzo un codice sconto Bottega Verde?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/bottegaverde.it), aggiungi i prodotti al carrello su Bottega Verde e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Bottega Verde?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Bottega Verde piu recenti?
La pagina [shopilo.it/negozi/bottegaverde.it](https://shopilo.it/negozi/bottegaverde.it) viene aggiornata quotidianamente con i codici sconto Bottega Verde, voucher Bottega Verde e coupon promozionali Bottega Verde piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Bottega Verde

Bottega Verde e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/bottegaverde.it) trovi i migliori codici sconto Bottega Verde, coupon Bottega Verde verificati e voucher Bottega Verde attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-bottegaverde
```

```javascript
const { fetchCoupons } = require('codice-sconto-bottegaverde');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
